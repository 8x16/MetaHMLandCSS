**FORM SUBMISSION**

Once we will the form and click on submit the form sends a HTTP request to the back end web server by the methods mentioned in the form element i.e. *GET* or *POST*

```html
<form action="#" method="get">
    <input type="text" name="username">
    <input type="password" name="password">
    <input type="submit" value="Submit">
</form>
```

Once we click submit, the above code results in URL being as follows:
```HTTP
https://www.domainname.com?username="valuesubmitted"&password="secret"
```

### Constraints of using GET in form submissions

1. All the data being submitted is visible in the URL even the passwords, so it is competely unsafe -> Security Threats
2. URL length is limited by the browsers (limit of around 2000 charcters by some browsers)
2. URL length is limited by web servers (NGINX has 4096 char as limit)

## Solution is to use POST method in form
```html
<form action="#" method="post">
    <input type="text" name="username">
    <input type="password" name="password">
    <input type="submit" value="Submit">
</form>
```

Once we click submit, the above code results in URL being as follows:
```HTTP
https://www.domainname.com/[actionelement]
```

The entire data is now carried as a body of the HTTP request but it can still be read by someone listening for the HTTP requests aka ***Man-In-the-Middle*** attacks

To get full security we use, encryption between the client and web server using HTTPS