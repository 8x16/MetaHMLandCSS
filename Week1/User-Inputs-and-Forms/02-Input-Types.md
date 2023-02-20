### Input Types

**Button**
displays a clicable button, and is mostly used in HTML forms to activate a script when clicked
```html
<input type="button" value="Click me" onclick="msg()">
```

We can also define the same functionality using the <code>&#60;button&#62;</code>tag

```html
<button onclick="alert('Are you sure you want to continue?')">
    <img src="https://yourserver.com/button_img.jpg" alt="Submit the form" height="64" width="64">
</button>
```

**Checkbox**
defines a checkbox allowing single values to be selected or deselected. They are used to let a user select one or more options of a limited number of choices
```html
<input type="checkbox" id="dog" name="dog" value="dog">
<label for="dog">I Like dogs</label>
<input type="checkbox" id="cat" name="cat" value="cat">
<label for="cat">I Like cats</label>
```

**Radio**
displays a radio button, allowing only a single value to be selected out of multiple choices
```html
<input type="radio" id="light" name="theme" value="Light">
<label for="light">Light</label>
<input type="radio" id="dark" name="theme" value="dark">
<label for="dark">Dark</label>
```

**Submit**
displays a submit button for submitting all values from an HTML form to a form-handler typically a server. The form-handler is specidied in the form's *"action"* attribute
```html
<form action="myserver.com" method="post">
...
<input type="submit" value="Submit">
</form>
```

**Text**
displays a basic single-line text field that a user can enter text into
```html
<label>First name:<input type="text" name="fname"></label>
```

**Password**
Defines a single-line text field whose value is obscured, suited for sensitive information like passwords
```html
<label>Password:
    <input type="password" name="pwd">
</label>
```

**Date**
Displays a control for entering date with no time(year, month and day)
```html
<label for="dob">Date of Birth</label>
<input id="dob" type="date" name="DOB">
```

**Datetime-local**
Displays a control for entering date and time, including year, month, day as wells as the time in hours and minutes
```html
<label for="birthdaytime">Birthday(date and time):</label>
<input id="birthdaytime" type="datetime-local" name="birthdaytime">
```

**Email**
Defines a field for an email address, similar to plain text input, with addition that it validates automatically when submitted to the server
```html
<label for="email">Enter your email:</label>
<input type="email" id="email" name="email">
```

**File**
Displays a control that lets the user select and upload a file from their computer. to define the types of files permissible you can use the "accept" atrribute. Also to enable multiple files to be selected, add the "multiple" attribute
```html
<label for="myFile">Select a file:</label>
<input type="file" id="myFile" name="myfile">
```

**Hidden**
Defines a control that is not displayed but whose value is still submitted to the server
```html
<input type="hidden" id="custId" name="custID" value="3487">
```

**Image**
Defines an image as a grahpical submit button. We should use "src" attribute to point to the location of your image files
```html
<input type="image" src="submit_img.png" alt="Submit" width="48" height="48">
```

**Number**
Defines a control for entering a number, You can use attributes to specify the restrictions, such as min and max values allowed, number  intervals or a default value
```html
<input type="number" id="quantity" name="quanity" min="1" max="5">
```

**Range**
Displays a range widget for specifying a number between two values, pricise value, however is not considered important, This is typically represented using a slider or dail control. To define the range use min and max attributes
```html
<label for="volume">Volume:</label>
<input type="range" id="volume" name="volume" min="0" max="10">
```

**Reset**
Displays a button that resets the contents of the form to their default values
```html
<input type="reset">
```

**Search**
Defines a text field for entering a search query. These are functionally identical to text inputs, but may be styles differently depending on the browser
```html
<input type="search" id="gsearch" name="gsearch">
```

**Time**
Displays a control for entering a time value in hours and minutes, with no timezone
<label for="appt">Select a time:</label>
<input type="time" id="appt" name="appt">

**Tel**
Defines a control for entering telephone number, we can optionally use the "pattern" field to perform validation
```html
<label for="phone">Enter your phone number:</label>
<input type="tel" id="phone" name="phone" pattern="[+]{1}[0-9]{11-14}">
```

**URL**
Displays a field for entering a text URL, It works similar to a text input, but performs automatic validation before being submitted to the server
```html
<label for="homepage">Add your homepage:</label>
<input type="url" id="homepage" name="homepage">
```

**Week**
Defines a control for entering a date consisting of a week-year number and a year with no timezone. Keep in mind that this is a newer type that is not supoorted by all the browsers
```html
<label for="week">Select a week:</label>
<input type="week" id="week" name="week">
```

**Month**
Displays a control for entering a month and a year with not time zone
```html
<label for="bdaymonth">Birthday(month and year):</label>
<input type="month" id="bdaymonth" name="bdaymonth" min="1930-01" value="2000-01">
```
