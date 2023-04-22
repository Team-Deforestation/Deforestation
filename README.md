Rules :

- Do not interact with someone else's files especially 
when we're working at the same time because you can cause merge conflicts
you can still view it though

- Be descriptive with your git commit message, if you just added css styling 
during your session, just write that.

- when you're done for the day, or gonna take a break, just push your code up
and tell others to git pull to pull your latest code.

- try your best not to use divs, use semantic html, 9 times out of ten you can
wrap an item with a <section> or <article> tag instead of div.

- Not everything needs a class or an ID, if you're trying to target something in a
container and you know it's the only elememt there just use css selectors
like if you're in the footer and you want to target a (p) element in the footer only
just do this :
                footer p {
                   Add styles
                }

- if you are going to use a class or id be specific with the naming convention
like if you need a class for a container holding an image call it :
class = "image-container".



- your html files should look like 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lusitana&family=Raleway&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css" type="text/css" />
    <title>Deforestation</title>
</head>

    <body>
        <header>
    
        </header>
    
        <main>
    
        </main>
    
        <footer>
    
        </footer>
    </body>
    
</html>


- your css files should start with 

* {
    margin: 0;
    padding: 0;
}

html {
    cursor: url('images/cursor.png'), auto;
}

body {
    font-family: 'Lusitana', sans-serif;
}

p {
    font-family: 'Raleway', serif;
}

/*header section*/


/*main section*/


/*footer section*/


/*media queries*/