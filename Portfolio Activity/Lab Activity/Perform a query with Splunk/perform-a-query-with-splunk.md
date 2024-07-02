# Activity: Perform a query with Splunk

## Activity Overview
In this activity, you'll be introduced to the Splunk platform. Then, you'll use Splunk Cloud to upload data, perform basic searches on the data, and answer a series of questions. Follow the instructions in the [Follow-along guide for Splunk sign-up](/Detection%20and%20Response/Module%204/follow-along-guide-for-splunk-sign-up.md) to complete the following before you begin using Splunk:

- Create a Splunk account

- Activate a free trial of Splunk Cloud

- Upload data into Splunk Cloud

> **Please note that this activity is optional and will not affect your completion of the course.**

So far, you've learned that SIEM tools, such as Splunk, are an important part of a security analyst's toolbox because they provide a platform for storing, analyzing, and reporting on data from different sources. You also explored some basic searches using Splunk's querying language, called Search Processing Language (SPL), which included the use of pipes and wildcards.

Creating effective searches is an important skill because it enables you to quickly and accurately find the information you are looking for within a large amount of data. Quick and accurate searching is especially useful during incident response, because you might need to swiftly identify and address a security incident. Effective search techniques also help you efficiently identify patterns, trends, and anomalies within data.

## Scenario
Review the following scenario. Then complete the step-by-step instructions.

You are a security analyst working at the e-commerce store Buttercup Games. You've been tasked with identifying whether there are any possible security issues with the mail server. To do so, you must explore any failed SSH logins for the root account.

> ***Note:** Use the incident handler's journal you started in [a previous activity](/Portfolio%20Activity/Documentation/Document%20an%20incident%20with%20an%20incident%20handler's%20journal/document-an-incident-with-an-incident-handler-s-journal.md) to take notes during the activity and keep track of your findings.*

## Step-By-Step Instructions
Follow the instructions and answer the following questions to complete the activity.

### Step 1: Access supporting materials
The following supporting materials will help you complete this activity. The data contains log and event information from Buttercup Games' mail servers and web accounts. This includes information like access and authentication logs, email logs, and more.

Link to supporting materials: [tutorialdata.zip](tutorialdata.zip) file

### Step 2: Create a Splunk Cloud account
To use Splunk Cloud, you must create an account. Follow *Part 1 - Create a Splunk Cloud account and Part 2 - Verify your email* in the [Follow-along guide for Splunk sign-up](/Detection%20and%20Response/Module%204/follow-along-guide-for-splunk-sign-up.md) to create an account.

### Step3 3: Sign up for a free Splunk Cloud trial
After you've created your Splunk account, you'll need to sign up for a free Splunk Cloud trial. Follow Part 3 - Activate a Splunk Cloud trial in the [Follow-along guide for Splunk sign-up](/Detection%20and%20Response/Module%204/follow-along-guide-for-splunk-sign-up.md).

> ***Note:**  you experience any issues activating your Splunk Cloud trial please check out the [Splunk cloud tutorial video](https://www.youtube.com/watch?v=5W7mzW8GATs&ab_channel=SplunkHow-To).*


### Step 4: Upload data into Splunk
To operate effectively, it's essential that SIEM tools ingest and index data. SIEM tools collect and process data so that it becomes searchable events that can be queried, viewed, and analyzed.

So far, you've created a Splunk account and activated and accessed the Splunk Cloud free trial, but your Splunk Cloud instance does not contain any data. Next, you'll need to upload data into Splunk to start querying. Complete the following steps to upload data into Splunk:

1. If you haven't already, download the data file from Step 1: [tutorialdata.zip](tutorialdata.zip). Click the link then click the download icon. Do not uncompress the file.

2. Navigate to Splunk Home from your Splunk Cloud free trial instance. You might need to log in again using your credentials from Step 3.

3. On the Splunk bar, click **Settings**. Then click the **Add Data** icon.

4. Click **Upload**.

5. Click the **Select File** button.

6. Upload the `tutorialdata.zip` file, and click **Open**.

7. Click the **Next** button to continue to **Input Settings**.

8. By the **Host** section, select **Segment in path** and enter **1** as the segment number.

9. Click the **Review** button and review the details of the upload before you submit. The details should be as follows: 

Input Type: Uploaded File

File Name: tutorialdata.zip

Source Type: Automatic

Host: Source path segment number: 1 

Index: Default

10. Click **Submit**. Once Splunk has ingested the data, you will receive confirmation that the file was successfully uploaded.

> ***Note:** you are experiencing issues uploading data into Splunk, refer to the [Splunk Search Tutorial](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/SearchTutorial/GetthetutorialdataintoSplunk) guide for help.*

### Step 5: Perform a basic search
Take a moment to examine the Splunk Cloud interface by locating the app panel, the Explore Splunk panel, and the Splunk bar.

![The Splunk home page for Splunk Cloud Platform displays the Apps panel, the Splunk bar and the Explore Splunk panel](/Portfolio%20Activity/img/the-splunk-home-page-for-splunk-cloud-platform-displays-the-apps-panel-the-splunk-bar-and-the-explore-splunk-panel.png)

Now that you've uploaded the data into Splunk, perform your first query to confirm that the data has been ingested, indexed, and is searchable. Follow these steps to perform a query:

1. Navigate to Splunk Home. (To return to Splunk Home, click the Splunk Cloud logo on the Splunk Cloud page.)
   
2. Click **Search & Reporting**. You may close any pop ups that appear.
   
3. In the search bar,  enter your search query:
`index=main`
This search term specifies the index. An **index** is a repository for data. Here, the index is a single dataset containing events from an index named main.

4. Select **All Time** from the time range dropdown to search for all the events across all time.

5. Click the search button. Note that the search button is represented by the magnifying glass icon. Your search should retrieve thousands of events.

![The Splunk Cloud search page displays the search bar and the time range drop down](/Portfolio%20Activity/img/the-splunk-cloud-search-page-displays-the-search-bar-and-the-time-range-drop-down.png)

> ***Pro tip:** It's a best practice to use short time ranges in your searches because a shorter time range returns results faster and uses fewer resources. Adjust the time using the time range dropdown or by using [time modifiers](https://docs.splunk.com/Documentation/SCS/current/Search/Timemodifiers) in your search.*

### Step 6: Evaluate the fields
When Splunk indexes data, it attaches fields to each event. These fields become part of the searchable index event data. This helps security analysts easily search for and find the specific data they need. Now that you've run your first query, examine the search results and the fields.

For each event the fields are `host`, `source`, and `sourcetype`. Under **SELECTED FIELDS**, examine the same fields.

![Splunk search results with the host, source, and sourcetype fields highlighted in red box](/Portfolio%20Activity/img/splunk-search-results-with-the-host-source-and-sourcetype-fields-highlighted-in-red-box.png)

Examine the field values by clicking on the field under **SELECTED FIELDS**. You should observe the following:

- **host:** The host field specifies the name of the network host from which the event originated. In this search there are five hosts:

    - `mailsv` - Buttercup Games' mail server. Examine events generated from this host
    - `www1` - This is one of Buttercup Games' web applications.
    - `www2` - This is one of Buttercup Games' web applications.
    - `www3` - This is one of Buttercup Games' web applications.
    - `vendor_sales`- Information about Buttercup Games' retail sales.

- **source:** The source field indicates the file name from which the event originates. You should identify eight sources. Notice `/mailsv/secure.log`, which is a log file that contains information related to authentication and authorization attempts on the mail server.

- **sourcetype:** The sourcetype determines how data is formatted. You should observe three sourcetypes. Examine `secure-2`.

### Step 7: Narrow your search
Because you've been tasked with exploring any failed SSH logins for the root account on the mail server, you'll need to narrow the search results for events from the mail server.

Under **SELECTED FIELDS**, click **host** and click **mailsv**.

Notice that a new term has been added to the search bar: `index=main host=mailsv`. The search results have narrowed to over 9000 events that are generated by the mail server.

### Step 8: Search for a failed login for root
Now that you've narrowed your search results to events generated by the mail server, continue to narrow the search to locate any failed SSH logins for the root account. 

1. Clear the search bar.

2. Enter `index=main host=mailsv fail* root` into the search bar. This search expands on the search from the previous task and searches for the keyword `fail*`. The wildcard tells Splunk to expand the search term to find other terms that contain the word *fail* such as *failure*, *failed*, etc. Lastly, the keyword `root` searches for any event that contains the term root.

3. Click **search**.

### Step 9: Evaluate the search results
Your search from the previous task should have retrieved search results for over 300 events. Navigate to other pages of the search results to observe the events not listed on the first page of results.

> ***Pro tip:** Splunk highlights search terms in search results to make it easier to identify where the search terms appear in the data.*

---

### Step 10: Answer questions about the search results 

1. How many events are contained in the main index across all time?
    
    a. 10,000

    b. Over 100,000

    c. 10-99

    d. 100-1,000

2. Which field identifies the name of a network device or system from which an event originates?

    a. source

    b. sourcetype

    c. host

    d. index

3. Which of the following hosts used by Buttercup Games contains log information relevant to financial transactions?

    a. vendor_sales

    b. www1

    c. www2

    d. www3

4. How many failed SSH logins are there for the root account on the mail server?

    a. None

    b. More than 100
    
    c. 100

    d. One

---

#### Key takeaways
In this activity, you used Splunk Cloud to perform a search and investigation. Using Splunk Cloud, you were able to:

- Upload sample log data 

- Search through indexed data

- Evaluate search results

- Identify different data sources 

- Locate failed SSH login(s) for the root account

If you would like to challenge yourself and explore more simulated incident investigations using Splunk, log in to Splunk and visit [Splunk Boss of the SOC](https://bots.splunk.com/).