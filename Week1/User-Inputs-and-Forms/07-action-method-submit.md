# Submit

We will see how submit works in this article.

## Action and Method

Forms are essential part of world wide web, nearly every website uses forms, from buying items online to ordering food for delivery. When we click the login button on a website, it sends your username and password to a web server to login to account.

we add a form to web page using form element
```html
<form></form>
```

but how the form is submitted is determined on two essential attributes: **action** and **method**

*action* attribute specifies to which web address the form must be sent. This address is the location of server-side code that weill process the request
```html
<form action="/login">
    <!-- Input fields go here -->
</form>
```

*It is important to note that action can be a full URL address such as <u>https://www.google.com/login</u>, or an absolute path such as <u>/login</u> or relative path such as <u>login</u>

Absolute path which starts with a forward slash, will use the base address of the current website, and combine it with the absolute path. 

Relative path will use the current address of the webpage

## METHODS

method specifies which HTTP method is used to submit the form: GET or POST

GET method (by default when it is not provided)
```html
<form method="get">

</form>
```

POST method
```html
<form method="post">

</form>
```

### NOTE ABOUT JSON

As we learn more about JS and front-end libraries, devs oftern submit the HTTP requests directly via code and send data as a part of the HTTP request body in a text format called JSON