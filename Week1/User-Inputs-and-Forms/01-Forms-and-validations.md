As a developer, we use HTML forms to capture user inputs, we must also ensure that the data is usable and is according to a specific format, that's where validations come in place.

**Form validation is a process that ensure that data is valid and conforms to defined rules by the developer**

There are two type of Validation
1. Client Side Validation - checks for errors as soon as they are typed in to the form, provides the user with immediate feedback
2. Server Side Validation - more secure as they prevent tampering and prevent invalid submissions. These checks can also perform more complex checks, like checking the data against a database or a business requirement

Most websites use both client-side and server-side validations to provide data integrity.

HTML allows us to do simple client side validation
```html
<!-- html has specific types of specific data types -->
<input type="email"> <!-- for email addresses -->
<input type="tel"> <!-- for telephone -->
<input type="url"> <!-- for URL -->
<input type="date"> <!-- for date values -->
<input type="time"> <!-- for time values -->
<input type="number"> <!-- for numeric values -->
<input type="range"> <!-- for numeric values which has min and max values -->
<input type="color"> <!-- for color selection -->


<!-- Another example is the required attribute, which indicates the user must supply value to an input field to allow for form submission -->
```