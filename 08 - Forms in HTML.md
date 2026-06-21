# 08 - Forms in HTML

## Introduction

HTML Forms are used to collect user input and send the entered data to a server for processing.

Forms are one of the most important features of web applications because they allow users to:

* Register accounts
* Login to applications
* Submit feedback
* Fill surveys
* Upload files
* Search information

HTML provides various form elements such as:

* `<form>`
* `<input>`
* `<label>`
* `<fieldset>`
* `<legend>`
* `<datalist>`
* `<option>`

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>HTML5 Forms Demo</title>
</head>
<body>

    <h2>User Registration Portal</h2>

    <form action="submit_handler.java" method="POST">

        <fieldset>

            <legend>Personal Credentials Data</legend>

            <p>
                <label for="username">Enter Full Name:</label>

                <input type="text"
                       id="username"
                       name="user_name"
                       required>
            </p>

            <p>
                <label for="userage">Enter Age:</label>

                <input type="number"
                       id="userage"
                       name="user_age"
                       required>
            </p>

            <p>
                <label for="useremail">Email Address:</label>

                <input type="email"
                       id="useremail"
                       name="user_email"
                       required>
            </p>

            <p>

                <label>Select Gender:</label><br>

                <input type="radio"
                       id="male"
                       name="gender"
                       value="M">

                <label for="male">Male</label>

                <input type="radio"
                       id="female"
                       name="gender"
                       value="F">

                <label for="female">Female</label>

            </p>

            <p>

                <label for="city_choice">
                    Select Cloud Platform Preference:
                </label>

                <input list="cloud_platforms"
                       id="city_choice"
                       name="preferred_cloud">

                <datalist id="cloud_platforms">

                    <option value="Microsoft Azure">

                    <option value="Amazon Web Services">

                    <option value="Google Cloud Platform">

                </datalist>

            </p>

            <p>

                <input type="checkbox"
                       id="terms"
                       name="agree_terms"
                       required>

                <label for="terms">
                    I accept the technical terms and conditions.
                </label>

            </p>

            <p>

                <input type="submit"
                       value="Register Account Data">

            </p>

        </fieldset>

    </form>

</body>
</html>
```

---

## 1. `<form></form>`

### Definition

The `<form>` tag is used to create an HTML form.

It acts as a container that holds all input controls.

### Syntax

```html
<form>

</form>
```

### Example

```html
<form action="submit_handler.java"
      method="POST">

</form>
```

---

### Action Attribute

The `action` attribute specifies where the form data should be sent.

Example:

```html
action="submit_handler.java"
```

---

### Method Attribute

The `method` attribute specifies how form data should be sent.

Two common methods:

* GET
* POST

Example:

```html
method="POST"
```

POST sends data securely in the request body.

---

## 2. `<input>`

### Definition

The `<input>` tag is used to receive user input.

It is an **unpaired tag**.

---

## Input Type: Text

```html
<input type="text">
```

Used to receive text from users.

Example:

```html
<input type="text"
       name="user_name">
```

---

## Input Type: Number

```html
<input type="number">
```

Used to accept numeric values.

Example:

```html
<input type="number"
       name="user_age">
```

---

## Input Type: Email

```html
<input type="email">
```

Used to accept email addresses.

Example:

```html
<input type="email"
       name="user_email">
```

The browser automatically validates email format.

---

## Input Type: Radio Button

```html
<input type="radio">
```

Used when the user can select only one option.

Example:

```html
<input type="radio"
       name="gender"
       value="M">

<input type="radio"
       name="gender"
       value="F">
```

---

## Input Type: Checkbox

```html
<input type="checkbox">
```

Used for accepting terms and conditions or selecting multiple options.

Example:

```html
<input type="checkbox"
       required>
```

---

## Input Type: Submit

```html
<input type="submit">
```

Creates a button to submit the form.

Example:

```html
<input type="submit"
       value="Register Account Data">
```

---

## 3. `<label></label>`

### Definition

The `<label>` tag provides a caption for an input element.

It improves:

* Accessibility
* User experience
* Screen reader support

### Example

```html
<label for="username">
Enter Full Name:
</label>
```

---

## 4. `<fieldset></fieldset>`

### Definition

The `<fieldset>` tag groups related form controls together.

It creates a border around form elements.

### Example

```html
<fieldset>

Form Elements

</fieldset>
```

---

## 5. `<legend></legend>`

### Definition

The `<legend>` tag defines a caption for the fieldset.

### Example

```html
<legend>
Personal Credentials Data
</legend>
```

Output:

```text
Personal Credentials Data
```

appears on the fieldset border.

---

## 6. `<datalist></datalist>`

### Definition

The `<datalist>` tag provides predefined suggestions for an input field.

### Example

```html
<datalist id="cloud_platforms">

<option value="Microsoft Azure">

<option value="Amazon Web Services">

<option value="Google Cloud Platform">

</datalist>
```

---

## 7. `<option>`

### Definition

The `<option>` tag defines an item inside:

* `<select>`
* `<datalist>`

### Example

```html
<option value="Microsoft Azure">
```

---

## Important Attributes

### required

Makes the field mandatory.

Example:

```html
required
```

---

### id

Provides a unique identifier.

Example:

```html
id="username"
```

---

### name

Specifies the variable name used when data is sent to the server.

Example:

```html
name="user_name"
```

---

## Explanation of the Program

This program creates a **User Registration Portal**.

It allows users to:

* Enter Full Name
* Enter Age
* Enter Email
* Select Gender
* Choose Cloud Platform
* Accept Terms and Conditions
* Submit the Form

---

## Important Points

* `<form>` creates a form.
* `<input>` accepts user input.
* `<label>` describes input fields.
* `<fieldset>` groups related controls.
* `<legend>` adds a title to the fieldset.
* `<datalist>` provides suggestions.
* `required` prevents empty submission.
* POST is commonly used to send sensitive form data.

---

## Summary

HTML Forms are one of the most important parts of modern web applications. They allow users to interact with websites by entering and submitting information. Tags such as `<form>`, `<input>`, `<label>`, `<fieldset>`, and `<datalist>` are fundamental building blocks for creating interactive and user-friendly web applications.
