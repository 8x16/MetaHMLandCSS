**Ensuring Non-Empty Fields**
By using *required* attribute
```html
<form action="/submit" method="post">
    <label>Email/Username:<br>
        <input type="email" name="email" placeholder="Enter your email or username" required>
    </label>
    <label>Password:<br>
        <input type="password" name="password" placeholder="Enter your password" required>
    </label>
    <input type="submit" value="Log-In">
</form>
```

**Ensuring the length of characters**
Length of input
```html
<form action="/register" method="post">
    <!-- Minimum length and Max Length -->
    <label>
        Username:
        <br>
        <input type="text" minlength="3" maxlength="12" required/>
    </label>
    <br>
    <label>
        Password:
        <br>
        <input type="password" minlength="8" maxlength="30" required/>
    </label>
    <br>
    <input type="submit" value="Register">
</form>
```

**Showing invalid data to users on Client**
We can use CSS :invalid pseudoselectors
```css
input:invalid {
    border: 1px solid red;
}

/* But the ablve code will show the fields red onLoad as the data is considered invalid on load, to avoid this */
input:focus:invalid {
    border: 1px solid red;
}
/* Above code works only when the user starts typing into the fields */
```