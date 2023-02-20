**Interactive Input Elements**
RADIO Buttons - only one selection

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <meta name="author" content="Pavan Kumar" />
        <meta name="description" content="Radio Buttons in HTML">

        <title>Radio Buttons</title>
    </head>
    <body>
        <header>
            <nav>
                <menu>
                    <li><a href="">Home</a></li>
                    <li><a href="">Blog</a></li>
                    <li><a href="">Contact</a></li>
                </menu>
            </nav>
        </header>
        <main>
            <h2>Book Table</h2>
            <form action="#" method="post">
                <fieldset id="size">
                    <!-- fieldset groups the input elements -->
                    <legend>Please select the size of the table</legend>
                    <label>
                        <input type="radio" name="size" value="2"> 2 person table
                    </label>
                    <label>
                        <input type="radio" name="size" value="4" checked> 4 person table
                    </label>
                    <label>
                        <input type="radio" name="size" value="6"> 6 person table
                    </label>
                </fieldset>
                <fieldset id="location">
                    <legend>Please select the location of the table</legend>
                    <label>
                        <input type="radio" name="location" value="indoor" checked> Indoor Table
                    </label>
                    <label>
                        <input type="radio" name="location" value="outdoor"> Outdoor table
                    </label>
                    <label>
                        <input type="radio" name="location" value="moonlight"> Moonlight/ Candle Light
                    </label>
                </fieldset>
                <button type="submit">Book table</button>
            </form>
        </main>
        <footer>
        </footer>
        <script src="./scripts/script.js">
        </script>
    </body>
</html>
```