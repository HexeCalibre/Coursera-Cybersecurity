# Assign Python variables

## Introduction
In this lab, you will open a notebook environment to practice assigning values to variables in Python. You’ll be presented with a security scenario to explore throughout the lab. You’ll create variables to keep track of information relevant to the login process for approved users to log in to a specific device.

## What you’ll do
You have multiple tasks in this lab:

- Assign variables of various data types

- Use the `type()` function to return a variable's data type

---

## Introduction

Variables help security analysts to keep track of a variety of security-related information. For example, analysts may need to create Python variables for the users who are allowed to log in, the number of login attempts that they're permitted, and the current number of attempts that a user has made.

In this lab, you'll practice assigning values to variables and determining their data types.

## Scenario
You are a security analyst who is responsible for writing code that will automate analysis of login attempts made to a specific device. As the first step, you'll need to create variables to keep track of information relevant to the login process. This information includes the device ID, list of approved usernames, maximum login attempts allowed per user, current login attempts made by a user, and login status.

Throughout this lab, you'll assign these variables and check the data types of the variables.

## ## Task 1
In your work as an analyst, imagine there is a device only users specified on an allow list can access, and its device ID is `"72e08x0"`.

In the following code cell, assign this value to a variable named `device_id`. Then, display the contents of the variable and observe the output.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign the `device_id` variable to the device ID that only specified users can access

device_id = ### YOUR CODE HERE ###

# Display `device_id`

print(### YOUR CODE HERE ###)
```

## Task 2
Now that the variable `device_id` is defined, you can return its data type.

In this task, use a Python function to find the data type of the variable `device_id`. Store the data type in another variable called `device_id_type`. Then, display `device_id_type` to examine the output.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign the `device_id` variable to the device ID that only specified users can access

device_id = "72e08x0"

# Assign `device_id_type` to the data type of `device_id`

device_id_type = ### YOUR CODE HERE ###

# Display `device_id_type`

print(### YOUR CODE HERE ###)
```

#### **Question 1**
**Based on the output above, what do you observe about the data type of `device_id`?**

```py
[Double-click to enter your responses here.]
```

## Task 3
As you continue your work, you're provided a list of usernames of users who are allowed to access the device. The usernames with this access are `"madebowa"`, `"jnguyen"`, `"tbecker"`, `"nhersh"`, and `"redwards"`.

In this task, create a variable called `username_list`. Assign a list with the approved usernames to this variable. Then, display the value of the `username_list` variable.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `username_list` to the list of usernames who are allowed to access the device

username_list = ### YOUR CODE HERE ###

# Display `username_list`

print(### YOUR CODE HERE ###)
```

## Task 4
In this task, find the data type of the `username_list`. Store the type in a variable called `username_list_type`. Then, display `username_list_type` to examine the output.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `username_list` to the list of usernames who are allowed to access the device

username_list = ["madebowa", "jnguyen", "tbecker", "nhersh", "redwards"]

# Assign `username_list_type` to the data type of `username_list`

username_list_type = ### YOUR CODE HERE ###

# Display `username_list_type`

### YOUR CODE HERE ###
```

#### **Question 2**
**Based on the output above, what do you observe about the data type of `username_list`?**

```py
[Double-click to enter your responses here.]
```

## Task 5
Now, imagine that you've been informed that the previous list is not up-to-date and that there is another employee that now has access to the device. You're given the updated list of usernames with access, including the new employee, as follows: `"madebowa"`, `"jnguyen"`, `"tbecker"`, `"nhersh"`, `"redwards"`, and `"lpope"`.

In this task, reassign the variable `username_list` to the new list. Run the code to display the list before and after it's been updated to observe the difference.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `username_list` to the list of usernames who are allowed to access the device

username_list = ["madebowa", "jnguyen", "tbecker", "nhersh", "redwards"]

# Display `username_list`

print(username_list)

# Assign `username_list` to the updated list of usernames who are allowed to access the device

### YOUR CODE HERE ### = ["madebowa", "jnguyen", "tbecker", "nhersh", "redwards", "lpope"]

# Display `username_list`

print(username_list)
```

#### **Question 3**
**Based on the output above, what do you observe about the contents of `username_list`?**

```py
[Double-click to enter your responses here.]
```

## Task 6
In this task, define a variable called `max_logins` that represents the maximum number of login attempts allowed per user. Store the value `3` in this variable. Then, store its data type in another variable called `max_logins_type`. Display `max_logins_type` to examine the output.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `max_logins` to the value 3

### YOUR CODE HERE ###

# Assign `max_logins_type` to the data type of `max_logins`

### YOUR CODE HERE ### = type(max_logins)

# Display `max_logins_type`

### YOUR CODE HERE ###(max_logins_type)
```

#### **Question 4**
**Based on the output above, what do you observe about the data type of `max_logins`?**

```py
[Double-click to enter your responses here.]
```

## Task 7
In this task, define a variable called `login_attempts` that represents the current number of login attempts made by a user. Store the value `2` in this variable. Then, store its data type in a variable called `login_attempts_type`. Display `login_attempts_type` to observe the output.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `login_attempts` to the value 2

### YOUR CODE HERE ###

# Assign `login_attempts_type` to the data type of `login_attempts`

### YOUR CODE HERE ###

# Display `login_attempts_type`

### YOUR CODE HERE ###
```

#### **Question 5**
**Based on the output above, what do you observe about the data type of `login_attempts`?**

```py
[Double-click to enter your responses here.]
```

## Task 8
In this task, you'll determine the Boolean value that represents whether the current number of login attempts a user has made is less than or equal to the maximum number of login attempts allowed.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.


```py
# Assign `max_logins` to the value 3

max_logins = 3

# Assign `login_attempts` to the value 2

login_attempts = 2

# Determine whether the current number of login attempts a user has made is less than or equal to the maximum number of login attempts allowed,
# and display the resulting Boolean value

print(### YOUR CODE HERE ### <= ### YOUR CODE HERE ###)
```

#### **Question 6**
**What is the output? What does this mean?**

```py
[Double-click to enter your responses here.]
```

## Task 9
This code continues to check for the Boolean value of whether `max_logins` is less than or equal to `login_attempts`. In this task, reassign other values to `login_attempts`. For example, you might choose a value that is higher than the maximum number of attempts allowed. Observe how the output changes.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `max_logins` to the value 3

max_logins = 3

# Assign `login_attempts` to a specific value

login_attempts = ### YOUR CODE HERE ###

# Determine whether the current number of login attempts a user has made is less than or equal to the maximum number of login attempts allowed,
# and display the resulting Boolean value

print(login_attempts <= max_logins)
```

#### **Question 7**
**Based on the different values you assigned to `login_attempts`, what did you observe about the output?**

```py
[Double-click to enter your responses here.]
```

## Task 10
Finally, you can also assign a Boolean value of `True` or `False` to a variable.

In this task, you'll create a variable called `login_status`, which is a Boolean that represents whether a user is logged in. Assign `False` to this variable and store its data type in a variable called `login_status_type` and display it.

Be sure to replace each `### YOUR CODE HERE ###` with your own code before you run the following cell.

```py
# Assign `login_status` to the Boolean value False

login_status = ### YOUR CODE HERE ###

# Assign `login_status_type` to the data type of `login_status`

login_status_type = type(login_status)

# Display `login_status_type`

print(login_status_type)
```

#### **Question 8**
**Based on the output above, what do you observe about the data type of `login_status`?**

```py
[Double-click to enter your responses here.]
```

## Conclusion

**What are your key takeaways from this lab?**

```py
[Double-click to enter your responses here.]
```