# CSS cheatsheet

## PROPERTIES
* **clip-path**
    * This property will clip the object borders according to the path given
    * It combines well with [polygon()](#polygon-function), circle(), path() or inset() functions
* **shape-outside**
    * This property will set the outside shape of an element

## FUNCTIONS
* **<a href="polygon-function"></a>polygon()**

## ANIMATION
* @keyframes

## Good Practices
* **Don't set root font size in absolute units**
    <br>This will prevent the user's browser settings, and i.e. visually
    <br>impaired users will not have the chance to change the font size on our page.
    <br>Default browser font size is usually 16px.
    <br>**USE PERCENTAGE WHEN CALCULATING THE ROOT FONT SIZE**
    <br>If 10px root font size is our initial intent then html's font-size value 
    <br>will be 62.5%. (Because 62.5% of 16 is 10).


## Examples
* Global reset example

            *,
            *::before,
            *::after {
                margin: 0;
                padding: 0;
                box-sizing: inherit;
            }
            
            html {
                font-size: 62.5%;
            }
            
            body {
                box-sizing: border-box;
            }
