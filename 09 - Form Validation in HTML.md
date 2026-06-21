# 09 - Form Validation in HTML

## Introduction

HTML5 provides built-in form validation features that help validate user input before submitting the form to the server.

Form validation helps to:

* Prevent invalid data entry
* Improve user experience
* Reduce server-side validation work
* Increase application security
* Ensure proper input format

HTML5 provides several validation attributes such as:

* `required`
* `placeholder`
* `pattern`
* `title`
* `min`
* `max`
* `maxlength`

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>HTML5 Username Validation Demo</title>
</head>
<body>

    <h2>Secure Account Access Portal</h2>

    <form action="validate_user.java" method="POST">

        <fieldset>

            <legend>Account Security Settings</legend>

            <p>

                <label for="username">
                    Create Username:
                </label>

                <input
                    type="text"
                    id="username"
                    name="user_name"
                    placeholder="ex: Apple123"
                    pattern="^[a-zA-Z0-9]{5,12}$"
                    title="Username must be alphanumeric and contain between 5 to 12 characters long."
                    required
                >

            </p>

            <p>

                <input type="submit"
                       value="Verify Credentials">

            </p>

        </fieldset>

    </form>

</body>
</html>
```

---

## Tags Used in this Program

### 1. `<form></form>`

#### Definition

The `<form>` tag is used to create a form that collects user input and sends it to the server.

#### Syntax

```html
<form action="server_file" method="POST">

</form>
```

#### Example

```html
<form action="validate_user.java"
      method="POST">

</form>
```

---

### Action Attribute

The `action` attribute specifies the destination where form data is sent.

Example:

```html
action="validate_user.java"
```

---

### Method Attribute

The `method` attribute specifies how form data is transmitted.

Common methods:

* GET
* POST

Example:

```html
method="POST"
```

POST is preferred for secure data transmission.

---

## 2. `<input>`

### Definition

The `<input>` tag accepts data from the user.

It is an unpaired tag.

---

## Input Type : Text

```html
<input type="text">
```

Used to accept text input.

Example:

```html
<input type="text"
       name="user_name">
```

---

## 3. Placeholder Attribute

### Definition

The `placeholder` attribute displays sample text inside the input box.

It disappears when the user starts typing.

### Example

```html
placeholder="ex: Apple123"
```

Output:

```text
ex: Apple123
```

appears as a hint inside the text field.

---

## 4. Pattern Attribute

### Definition

The `pattern` attribute is used to validate input using a Regular Expression (Regex).

If the entered value does not match the pattern, the form will not be submitted.

---

### Pattern Used

```html
pattern="^[a-zA-Z0-9]{5,12}$"
```

---

### Meaning of the Pattern

| Expression | Meaning                             |
| ---------- | ----------------------------------- |
| ^          | Beginning of text                   |
| a-z        | Lowercase letters                   |
| A-Z        | Uppercase letters                   |
| 0-9        | Digits                              |
| {5,12}     | Minimum 5 and maximum 12 characters |
| $          | End of text                         |

---

### Valid Usernames

```text
Apple123
Java2025
HTMLUser
Code99
```

---

### Invalid Usernames

```text
ab
apple@
my username
1234567890123456
```

Reasons:

* Too short
* Contains special characters
* Contains spaces
* Exceeds maximum length

---

## 5. Title Attribute

### Definition

The `title` attribute displays an error message or hint when validation fails.

### Example

```html
title="Username must be alphanumeric and contain between 5 to 12 characters long."
```

If the user enters invalid data, this message is displayed automatically by the browser.

---

## 6. Required Attribute

### Definition

The `required` attribute makes an input field mandatory.

The form cannot be submitted until a value is entered.

### Example

```html
required
```

---

## 7. `<fieldset></fieldset>`

### Definition

The `<fieldset>` tag groups related form controls together.

It creates a border around the form section.

### Example

```html
<fieldset>

Form Controls

</fieldset>
```

---

## 8. `<legend></legend>`

### Definition

The `<legend>` tag defines a title for the fieldset.

### Example

```html
<legend>
Account Security Settings
</legend>
```

Output:

```text
Account Security Settings
```

appears on the fieldset border.

---

## 9. Submit Button

```html
<input type="submit"
       value="Verify Credentials">
```

### Definition

The submit button sends form data to the server after successful validation.

Output:

```text
Verify Credentials
```

---

## Program Flow

```text
User Opens Form

↓

Enter Username

↓

Browser Checks:
- Required?
- Length between 5 and 12?
- Only letters and digits?

↓

If Valid
Submit Form

↓

If Invalid
Display Validation Message
```

---

## Important Points

* HTML5 provides built-in validation.
* `required` prevents empty submission.
* `placeholder` provides sample input.
* `pattern` validates data using Regular Expressions.
* `title` displays validation messages.
* Validation improves security and user experience.
* Browser validation reduces unnecessary server requests.

---

## Advantages of HTML5 Validation

1. Simple to implement.
2. No JavaScript required.
3. Faster validation.
4. Better user experience.
5. Reduces invalid submissions.
6. Improves application security.

---

## Summary

HTML5 Form Validation provides powerful built-in features to validate user input before sending it to the server. Attributes such as `required`, `placeholder`, `pattern`, and `title` help developers create secure, user-friendly, and professional web forms with minimal code.
