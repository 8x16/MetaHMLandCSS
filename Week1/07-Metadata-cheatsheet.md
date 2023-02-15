**HTML <code>&#60;meta&#62;</code> tags**

STRUCTURE

For Author
```html
<meta name="author" content="Pavan Kumar">
```

For Content
```html
<meta name="language" content="english">
```

For Charset
```html
<meta charset="UTF-8">
```

For HTTP-equiv

This field stands for HTTP equivalent, and it is used to stimulate HTTP response headers. This is rare to see and it is recommended to use HTTP headers over HTML http-equiv meta tags.

For example, we can specify a header that instruct the browser to refesrh the page every 30 minutes
```html
<meta http-equiv="refresh" content="30">
```

### BASIC META TAGS FOR SEO
```html
<meta name="description" content="provides a brief description of the web page"/>

<meta name="title" content="specifies the title of the web page">

<meta name="author" content="specifies the author of the web page">

<meta name="language" content="specifies the language of the web page">

<meta name="robots" content="index, follow" /> <!-- Tells all the search engines how to crawl or index a certain page -->

<meta name="googlebot" content="index, follow" /> <!-- Tells only the google search engine how to crawl or index a certain page -->

<meta name="googlebot" content="notranslate" /> <!-- Tells google not to provide an automatic translation for your page if the user uses a different language -->

<meta name="google" content="nositelinksearchbox"/> <!-- Tells google not to show the sitelinks searchbox for our page when showing seartch results -->

<meta name="rating" content="safe for kids"> <!-- specifies the expected audience for your page -->

<meta name="copyright" content="Copyright 2023"> <!-- Specifies a copyright -->

<meta name="revised" content="Sunday, July 18th, 2022, 5:15 pm"> <!-- specifies the last modified date and time of changes-->
```

### META HTTP-EQUIV

These tags are used to set headers properties that browser will use, usually these are set by the back end server not in the files
```html
<meta http-equiv="content-type" content="text/html"> <!-- Specifies the format of the document returned by the server --> 

<meta http-equiv="default-style" > <!-- specifies the format of styling the document -->

<meta http-equiv="Content-language" content="english">

<meta http-equiv="Cache-control" content="no-cache"> <!-- instructs the browser how to cache our page>
```

### RESPONSIVE DESIGN/MOBILE META TAGS
For usage on Mobiles and non-desktop devices
```html
<meta name="format-detection" content="telelphone=yes"> <!-- Indicates the telephone numbers should appear as hypertext links that can be clicked to make a phone call -->

<meta name="HandheldFriendly" content="true"> <!-- specifies that the page can be properly visualized on mobile devices -->

<meta name="viewport" content="width=device-width, intial-scale=1.0"> <!-- specifies the area of the window in which web content can be seen -->
```