# How to Use

Go to my [Github Pages website](http://ashleydonohoe.github.io/) to access index.html.
Click the "Cam's Pizzeria" link to go to pizza.html.

# Optimizations Made

#The following changes were made to [index.html](http://ashleydonohoe.github.io/) to achieve a page score above 90:

Minified the CSS

Removed the external font from CSS and HTML

Moved the JS files to the end of the document and used "async" on them

Specified print.css as the print media type

Compressed pizzeria and profilepic to make them much smaller; used Google's suggested optimized versions

Resized pizzeria image to 100px since that was the largest size it appeared

Incorporated the loadCSS function from https://github.com/filamentgroup/loadCSS/blob/master/loadCSS.js to asynchronously load the CSS


#The following changes were made to achieve 60 FPS for [pizza.html](http://ashleydonohoe.github.io/views/pizza.html):

Updated the updatePositions function to hold all the 'mover' class items in an array outside the for loop and to use just six columns of pizzas with a total of 24. 200 pizzas on 8 rows isn't necessary since many of them aren't even above the fold on the page and in view

Applied backface-visibility:hidden; in the CSS for the 'mover' class

I regrouped the newsize and dx variables to go in the DetermineDX function

Replaced var windowwidth = document.querySelector("#randomPizzas").offsetWidth; with var windowwidth = document.getElementById("randomPizzas").offsetWidth; to get the elements more quickly by ID. I did the same with the selectors for the pizzaSize ID in the changeSliderLabel function.

Resized and compressed the pizza and pizzaria images

Minified the CSS files


