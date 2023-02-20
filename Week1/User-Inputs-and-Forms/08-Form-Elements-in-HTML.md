## INPUT

It is used to create interactive controls, and validation of user inputs. the key attribute of this element is <u>type</u> which include values like *text, password, button, checkbox, radio, date, email, number, submit, url, datetime-local etc*

They control the appearance and also the validations of the input fields

```html
<form action="/login" method="post">
    <label>
        Username:
        <br>
        <input type="text" id="uname" name="username" required>
    </label>
    <label>
        Password:
        <br>
        <input type="password" id="password" name="password" required>
    </label>
    <input type="submit" value="Login">
</form>
```

## LABEL

Defines a label for an input element and increases the clickable area of an associated input element, it can be associated by nesting or using "for" attribute

Let's look at the same above example, using various label ways
```html
<form action="/login" method="post">
    <!-- Nesting under label -->
    <label>
        Username:
        <br>
        <input type="text" id="username" name="username" required>
    </label>
    <br>
    <!-- Using 'for' attribute -->
    <label for="password"></label>
    <input type="password" id="password" name="password" required minlength="8" pattern="{A-Za-Z}[0-9]">
</form>
```

## SELECT

Defines a drop-down list of options presented to the user, It has couple of attributes:
* Form, the id of the form in which the drop-down appears
* Name specified the name of the control
* Multiple boolean attribute, when specified, indicates if a user can select multiple options out of the list
* Required boolean attribte, indicates if the field is mandatory
* size mentions the number of visible options in a drop-down list

Options in the dropdown are defines using the <code>&#60;option&#62;</code> element inside the <code>&#60;select&#62;</code>

### OPTION

Defines an option for the dropdown list, To pre-select an option use *selected* on option

```html
<form action="/login" action="post">
    <label> How did you hear about us?: 
        <select name="promoters" size="3" multiple required>
            <option value="Online Ads"></option>
            <option value="Friend"></option>
            <option value="Bonus"></option>
            <option value="Didn't hear"></option>
            <option value="Returning User"></option>
        </select>
    </label>
</form>
```

### OPTGROUP

Group Options with headings, use *label" attribute to specify the option group heading
```html
<form action="/login" action="post">
    <label> How did you hear about us?: 
        <select name="promoters" size="3" multiple required>
            <optgroup label="Online">
                <option value="Online Ads">Online</option>
                <option value="Friend">Friend</option>
                <option value="Bonus">Bonus</option>
            </optgroup>
            <optgroup label="Offline">
                <option value="Didn't hear">Never Heard</option>
                <option value="Returning User">Already used it</option>
            </optgroup>
        </select>
    </label>
</form>



## TEXTAREA

To enter rich text, typically to allow the user to input longer textual data. The common attributes for this element include:
* cols, defines the width of the text area, default is 20
* form, the form element the text area is linked with
* maxlength, max numbers of chracters that can be entered in the text area
* minlength, min numbers of characters that the user should enter
* readonly, once set the user cannot modify the contents
* rows, defines the numbers of visible text lines for the text area

```html
<textarea name="response" rows="10" cols="30" maxlength="200">

</textarea>
```

## BUTTON

Defines a clickable button, onlick attribute defines the behaviour when the button is clicked by the user
```html
<button onclick="alert(`You just clicked Me!!!`)">Click Me!</button>
```

## FEILDSET

Group related input elements in a form, elements realted ti personal info, and education qualifaction can be gripued seperately in two field sets

### LEGEND

Defines a caption for the *'filedset'* element
```html
<fieldset> 
  <legend>Personal Info</legend> 
  <label for="fname">First name:</label><br> 
  <input type="text" id="fname" name="fname" value="John"><br> 
  <label for="lname">Last name:</label><br> 
  <input type="text" id="lname" name="lname" value="Doe"><br> 
</fieldset> 

<fieldset> 
  <legend>Qualificaiton</legend> 
  <label for="pdegree">Primary degree:</label><br> 
  <input type="text" id="pdegree" name="degree" value="Masters"><br> 
  <label for="fos">Last name:</label><br> 
  <input type="text" id="fos" name="field" value="Psychology"><br> 
</fieldset> 
```


## DATALIST

Specifies a list of pre-defined options for an input element.

**It defers from <code>&#60;select&#62;</code> since the user can still provide textual ot numeric input other than listed options** 

```html
    <input list="flowers" name="flowers">
    <datalist id="flowers">
        <option value="Rose">
        <option value="Lily">
        <option value="Tulip">
        <option value="Daffodil">
        <option value="Orchid">
    </datalist>
```

## OUTPUT

It represents the result of a calculation(typically the output of a script) or the outcome of an user action

```html
<input type="range" name="people_attending" min="4" max="10" step="0.5" oninput="this.nextElementSibling.value = this.value">
<output>4</output>
```

