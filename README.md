Animate Numbers jQuery Plugin
===============

Apply this plugin to an element that contains a number and it will animate to the new number you specify. Works with appropriate inputs.

Note: once an input has been animated refreshing the page will not trigger the inputs to animate again. This is due to browsers maintaining input values after reload. You will have to manually change the value and trigger the animation again.

Examples
---------------

**HTML:**

&lt;div id="num"&gt;1234&lt;/div&gt;

**JS:**

$("#num").animateNumbers(4321);

In this example the div #num will be animated from 1234 to 4321 using the defaults; one second, with commas, swing ease.

The other extreme is to set the options to something other than the defaults.

**HTML:**

&lt;div id="num"&gt;1234&lt;/div&gt;

**JS:**

$("#num").animateNumbers(4321, false, 2000, "linear");

Here's an example of a number input:

**HTML:**

&lt;input type="number" id="num_input" value="1234" /&gt;

**JS:**

$("#num_input").animateNumbers(4321);

In this example the div #num will be animated from 1234 to 4321 with these settings: two seconds, no commas, linear ease.

Most likely you will apply the plugin method to an element upon an event firing. Document ready and click are common choices.

Demo
---------------

http://jsfiddle.net/JsEa6/267/

Notes
---------------

This plugin uses the $.animate() method of jQuery to step a number towards the desired number. I got the idea from here:

http://www.josscrowcroft.com/2011/code/jquery-animate-increment-decrement-numeric-text-elements-value/

I extended the example to what I have here to suit a project of mine. Decided to put it up on GitHub in case someone else finds it useful.

If the end result number is to have commas then it is suggested that the number created in HTML have commas as well.
