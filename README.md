less-scss-tutorial
==================

Tutorial about how to use LESS

For information about LESS and its advantages and a complete list of all features please visit https://github.com/cloudhead/less.js

Descriptions about what happens in the single steps and how it is done will follow

## GOAL ##

Our goal is as follows:
 - The Web-Page should be centered within the available space in the window.
 - It should scale with the window size (down to a certain boundary)
 - The web page should be responsive
 -- On 'normal' devices with a mouse, detail information to a person should be gained via hovering of the appropriate picture
 -- When the available space grows less, the amount of columns shown should be reduced
 -- The headline should change it's size accordingly
 -- The headline subtitle ('Software is our passion') should vanish if there isn't enough space anymore
 -- If the available resolution indicates a mobile device the person detail text should always be shown (as no hover is possible)
 - It should be easy to change certain aspects of our styling
 -- Colors, Font types, etc. should be changeable in a single location

## INIT ##

The base of our tutorial. The html file shows our basic web structure:
 - header
 -- headline
 -- menu
 - content
 -- list of persons
 - footer

If opened in a browser one can see that no styling has been applied and that it looks quite unusable.
We will change that within the next few steps of our tutorial.

## STEP 1 ##

Lets start with our global layout:

First we define our css rules which will apply to the body and other general settings:

    body {
		font-family: Helvetica, Arial, sans-serif;
		width: 80%;
		max-width: 960px;
		margin: 0 auto;
		border: 1px solid red;
		background: #fafafa;
    }

We just defined our font-family for the whole page, and some basic styling properties:

 - Our whole page uses only 80% of the available window width
 - When the window grows larger, we don't scale up infinetely - we stop at 960px
 - the margin rule tells our body to be centered inside the window
 - the border is just here to make the 80% / max-width settings more eveident for the moment
 - a background for our body in a light grey is defined

So far nothing different then plain css has been written, but we will change this just in a few moments.

TODO
...