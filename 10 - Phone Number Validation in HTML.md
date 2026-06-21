# 10 - Phone Number Validation in HTML

## Introduction

HTML5 provides built-in validation features to verify user input before submitting data to the server.

Phone number validation is one of the most common validations used in:

* Registration Forms
* Banking Applications
* E-Commerce Websites
* Social Media Applications
* Contact Forms
* Employee Management Systems

HTML5 provides the following attributes to validate phone numbers:

* `type="tel"`
* `placeholder`
* `pattern`
* `title`
* `required`

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>HTML5 Phone Validation Demo</title>
</head>
<body>

    <h2>Contact Information Verification</h2>

    <form action="save_contact.java" method="POST">

        <fieldset>

            <legend>Communication Details</legend>

            <p>

                <label for="phone">
                    Mobile Number:
                </label>

                <input
                    type="tel"
                    id="phone"
                    name="user_phone"
                    placeholder="Ex: 9876543210"
                    pattern="^[0-9]{10}$"
                    title="Please enter a valid 10-digit mobile number containing only numbers."
                    required
                >

            </p>

            <p>

                <input type="submit"
                       value="Submit Contact Record">

            </p>

        </fieldset>

    </form>

</body>
</html>
```

---

## Tags and Attributes Used

### 1. `<form></form>`

#### Definition

The `<form>` tag is used to collect user input and send the entered data to the server.

#### Syntax

```html
<form action="server_file" method="POST">

</form>
```

#### Example

```html
<form action="save_contact.java"
      method="POST">

</form>
```

---

### Action Attribute

The `action` attribute specifies where the form data will be sent after submission.

Example:

```html
action="save_contact.java"
```

---

### Method Attribute

The `method` attribute specifies how the form data is transmitted.

There are two common methods:

* GET
* POST

Example:

```html
method="POST"
```

POST sends the form data securely through the request body.

---

## 2. Input Type : Tel

### Definition

The `type="tel"` input is used for entering telephone or mobile numbers.

Syntax:

```html
<input type="tel">
```

Example:

```html
<input type="tel"
       name="user_phone">
```

---

## 3. Placeholder Attribute

### Definition

The `placeholder` attribute displays sample text inside the input field.

It disappears automatically when the user starts typing.

Example:

```html
placeholder="Ex: 9876543210"
```

Output:

```text
Ex: 9876543210
```

---

## 4. Pattern Attribute

### Definition

The `pattern` attribute validates the entered value using a Regular Expression (Regex).

If the value does not match the pattern, the browser prevents form submission.

Example:

```html
pattern="^[0-9]{10}$"
```

---

### Explanation of the Pattern

| Pattern | Meaning            |
| ------- | ------------------ |
| ^       | Beginning of input |
| [0-9]   | Digits from 0 to 9 |
| {10}    | Exactly 10 digits  |
| $       | End of input       |

---

### Valid Mobile Numbers

```text
9876543210
9988776655
7894561230
```

---

### Invalid Mobile Numbers

```text
98765
98765432101
98765abcde
98 76543210
```

Reasons:

* Less than 10 digits
* More than 10 digits
* Contains alphabets
* Contains spaces

---

## 5. Title Attribute

### Definition

The `title` attribute displays a helpful validation message when the input is invalid.

Example:

```html
title="Please enter a valid 10-digit mobile number containing only numbers."
```

If validation fails, the browser automatically shows this message.

---

## 6. Required Attribute

### Definition

The `required` attribute makes the field mandatory.

The form cannot be submitted unless the user enters a valid value.

Example:

```html
required
```

---

## 7. `<fieldset></fieldset>`

### Definition

The `<fieldset>` tag groups related form controls inside a bordered box.

Example:

```html
<fieldset>

Form Controls

</fieldset>
```

---

## 8. `<legend></legend>`

### Definition

The `<legend>` tag provides a title for the fieldset.

Example:

```html
<legend>
Communication Details
</legend>
```

Output:

```text
Communication Details
```

This text appears on the fieldset border.

---

## Program Flow

```text
User Opens Form

↓

Enter Mobile Number

↓

Browser Checks:

- Field is empty?
- Contains exactly 10 digits?
- Contains only numbers?

↓

If Valid

Submit Form

↓

If Invalid

Display Validation Error Message
```

---

## Advantages of Phone Validation

1. Prevents invalid phone numbers.
2. Improves data accuracy.
3. Enhances user experience.
4. Reduces server-side validation.
5. Helps maintain clean database records.
6. Improves application reliability.

---

## Important Points

* `type="tel"` is used for phone number input.
* `pattern` validates the format using Regex.
* `placeholder` displays sample input.
* `required` prevents empty submission.
* `title` displays custom validation messages.
* HTML5 validation works without JavaScript.

---

## Summary

HTML5 Phone Number Validation allows developers to validate mobile numbers directly in the browser using built-in attributes such as `type="tel"`, `pattern`, `required`, and `title`. It improves data quality, enhances user experience, and reduces unnecessary server-side validation, making forms more secure and professional.

---
