# Simple-grid



A simple 12 columns, responsive CSS grid that includes [**Normalize.css**](https://github.com/necolas/normalize.css/)

For some projects I was using Bootstrap only for the grid system, so I decided to make my own inspired in Bootstrap grid.  


## Usage  
Load the simple-grid.css or simple-grid.min.css in your document
```HTML
<link rel="stylesheet" href="css/simple-grid.css">
```

To effectively use the grid, first, you need to define a row using the row class, then you can define the amount of columns
that an element will occupy. Note that you can nest columns to create interesting layouts (See the demos).

The small size is considered the base size, so you always need to define, at least, that size for your element.
The classes used to define the columns start with "col-" followed by the size (xs-, sm-, md-, lg-) and then, 
the number of columns (1 to 12). 

For example:
  
- **col-sm-9** = Nine columns in a small screen size
- **col-md-4** = Four columns in a medium screen size
- **col-lg-6** = Six columns in a large screen size
- **col-xs-12** = Twelve columns in a extra small screen size

The breakpoints are defined as:

- **Large (lg)**: Screen > 768px
- **Medium (md)**: Screen between 550px and 768px
- **Small (sm)**: Screen between 450px and 550px
- **Extra small (xs)**: Screen < 450px

An example of the HTML marking: the content will occupy a different amount of columns depending on the screen size
```HTML
<div class="row">
    <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3>
        --- Content ---
    </div>
</div>
```


## Some utilities

By defaut, the grid sets the text decoration of links to none. Also, images are set by default to have a 100% width 
and vertical-align: top (You can change it if you need/want).

There are two extra classes included:
- **pd-fix**: Sets padding to 0, useful when nesting columns (see the demo 4).
- **container**: Automatically center the elements in the documment.
