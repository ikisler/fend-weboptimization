# Portfolio and Pizzeria Website Optimization
###Original code by Cameron Pittman at Udacity, optimizations enacted by Isabeau Kisler

###The Project
Optimized an inefficient web application's JavaScript, CSS and assets delivery, ensuring it runs at 60fps and achieves a PageSpeed score of 95.

## Portfolio Optimizations:
* Minify and inline the main CSS
* Add 'media="print"' for the CSS file dedicated to printing the page
* Add ASYNC to the <script> tags, and move them to the end of <body>
* Remove nonfunctional font link
* Resize and compress images

## Pizzeria Optimizations:
* changePizzaSizes function: Integrate determineDX into changePizzaSizes function, remove the For loop and add CSS classes to control random pizza sizes.  The pizza size is then changed all at once for all pizzas, rather than iterating through the entire list
* updatePositions function: Create the array of background pizzas outside the function and calculate the phase numbers outside of the function, as these events only need to happen once, not every time the function is called
* Change the number of background pizzas ('.mover') to 35, down from 200
* Add 'will-change' to '.mover' and '.randomPizzaContainer'

###Running the Program
To launch the websites, download the files from Github, then double-click on 'index.html' for the portfolio site, or navigate to the 'views' folder and double-click on the 'pizza.html' file for the pizzeria site.  The pizzeria site is also accessible by going through the portfolio website.
