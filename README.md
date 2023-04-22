Rules :

- Do not interact with someone else's files especially 
when we're working at the same time because you can cause merge conflicts
you can still view it though
nathaniel: about.html about.css   meetUs.html meetUs.css
marcus: donate.html donate.css

- Be descriptive with your git commit message, if you just added css styling 
during your session, just write that.

- when you're done for the day, or gonna take a break, just push your code up
and tell others to git pull to pull your latest code.

- try your best not to use divs, use semantic html, 9 times out of ten you can
wrap an item with a <section> or <article> tag instead of div. you can target
an element using nth of child too, use can use divs if something is very nested

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


Nav html: 

<header>
        <nav>
            <div>
                <figure><img src="images/deforestation.png"></img></figure>
                <h2>Deforestation</h2>
            </div>
            <input type="checkbox" id="check" />
            <label for="check" class="burger-icon">
                <img src="images/burger-bar.png"></img>
            </label>
            <ul>
                <li id="home-underline"><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="donate.html">Donate</a></li>
            </ul>
        </nav>
</header>

nav css :

* {
    margin: 0;
    padding: 0;
}

:root {
    --nav-bg-color: #435944;
    --beige-color: #CAB170;
}

html {
    cursor: url('images/cursor.png'), auto;
}

body {
    font-family: 'Lusitana', sans-serif;
}

p,
a {
    font-family: 'Raleway', serif;
}

/*header section*/

header {
    background-color: var(--nav-bg-color);
    color: white;
    padding: 1.4rem 1.6rem;
    position: sticky;
    top: 0;
    font-size: 1.2rem;
}

nav {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

nav :nth-child(1) {
    display: flex;
    gap: 20px;
    align-items: center;
}

nav div :nth-child(1) {
    width: 45px;
    height: 45px;
}

nav :nth-child(4) {
    display: flex;
    gap: 2rem;
    list-style: none;
    align-items: center;
}

#home-underline {
    text-decoration: underline;
}

.burger-icon {
    cursor: pointer;
    display: none;
}

.burger-icon :nth-child(1) {
    width: 40px;
    height: 40px;
}

#check {
    display: none;
}

a {
    font-size: 1.06rem;
    text-decoration: none;
    color: white;
    transition: color 0.4s ease;
}

a:hover {
    color: var(--beige-color)
}


/*main section*/


/*footer section*/


/*media queries*/

@media (min-width: 580px) {
    #check:checked~ul {
        display: flex;
        gap: 2rem;
    }
}

@media (max-width: 580px) {
    header {
        padding: 0.8rem 0.8rem;
    }

    nav :nth-child(4) {
        display: none;
        width: 100%;
        padding: 1.3rem 0;
    }


    li {
        text-align: center;
    }
    
    #check:checked~ul {
    display: flex;
    flex-direction: column;
    
}


    .burger-icon {
        display: block;
    }

}
