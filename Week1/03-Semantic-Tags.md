When we write content it is best to convey the semantics(meaning), this allows search engines and accessibility softwares to understand the contents of a page

We can easily do this using tags, for example <code>h1</code>...<code>h6</code> tags for headings, similarly the <code>ul</code> and <code>ol</code> tags to convey that they are **unordered** and **ordered** lists respectively

### BASIC STRUCTURE OF A HTML PAGE
```html
<!DOCTPYE html>
<html>
    <head>
        <meta charset="UTF-8" />
    </head>
    <body>
        <!-- Inside the body, we can layout the website with very semantic tags to describe each of the sections -->
        <header>
            <nav>
                <!-- Main Navigation Section of the webpage -->
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </header>
        <main>
            <!-- Two main semantic elements for the content are article and section, they are nested under each other by some developers -->
            <section>
                <article>
                    <h2>Heading for the article</h2>
                    <p>According to the World Wide Web Consortium's website, the article element indicates content which represents a complete. Or self contained composition in a document page application or site that is independently distributable.</p>
                </article>
            </section>
            <article>
                <section>
                    semantically define the individual sections of the article, sections should / could also contain heading elements to sementically define the section

                    we can also use sections to describe different elements of the webpage like Biodata, Tech Data etc in a portifolio
                </section>
            </article>
            <aside>
            <aside>
        </main>
        <footer>
            <!-- Can also include contact info and social media links -->
            <address>
            </address>
        </footer>

    </body>
</html>
```