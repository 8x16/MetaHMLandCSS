<!-- When we share a link of the website on a social app most create a preview of the link -->
<!-- we can control what info is displayed on these social sites to get more links -->

<!-- different from traditional meta tags used for SEO -->
<!-- Traditional SEO tags are used for search results not direct links -->
<!-- Facebook due to its popularity created Open Graph Protocol in 2010 -->

<!-- It is a set of meta data rules that allowed webpages to that allowed webpages to describe themselves to social networks -->

<!-- Many meta data tags available within the protocol -->

### META TAGS
```html
<head>
    <!-- Standard HTML meta tags for SEO -->
    <meta name="author" content="John Doe">

    <!-- Open Graph Meta tags for Social apps -->
    <meta property="og:title" content="My First Web page" />
    <!-- meta tage name is replaced with property, to distinguish it more the value for name starts with og: to indicate open graph protocol -->

    <!-- OG Protocol indicates that we must always include 4 properties in a webpage -->
    <meta property="og:title" content="My First Web page" />
    <!-- Defines the title of the page that appears in the preview -->
    <meta property="og:type" content="website"/>
    <!-- Type of content such as website, audio, video, article -->
    <meta property="og:url" content="https://www.example.com/"/>
    <!-- Permanent web address for the page -->
    <meta property="og:image" content="https://www.example.com/me.jpg"/>
    <!-- An image that must be displayed when the website is shared -->

    <!-- Several other properties are also present, few are -->
    <meta property="og:description" content="John's first web page"/>

    <meta property="og:locale" content="en_US">
    <!-- locale displays, language and territory -->

    <meta property="og:site_name" content="John's website">
    <!-- Overall name of the website -->
</head>
```