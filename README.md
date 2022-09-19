# Rothko-Painting

Add a div element with class "canvas"
use div's class selector to select it in the css file and give a width of 500px.
add height property in the canvas class selector and give it a value of 600px.
add background color to canvas class selector with a value of #4d0f00
as every paiting needs a frame, put canvas div inside frame div
now we can add border with div's class frame
observe that frame's boundary is much wider than the canvas.In frame class selector, give a width of canvas width which is 500px.
in frame class selector, give a padding of 50px on all 4 sides of it, it will give a space of 50px on all sides between frame and canvas
use margins to to adjust the spacing outside of an element, give frame class selector a margin of 20px top and bottom and auto to left and side.
top and bottom margin of 20px will leave space of 20px at the top and bottom.
auto margin at left and right side will leave space eually from left and right side according to the available space, in this case, it will center the div element and the child elements too.
Add a new div element inside .canvas and give it as class of one
use .one to select the new div's class and give it a width of 425px.
give .one selector a height of 150px and background color of #efb762. Now a rectanlge will appear inside canvas div of diemnsion of 425px width and 150px height.
give margin to .one class of 20px top and bottom and left and right with auto, what it will do is, it will make space of 20px on top and bottom by pushing it downward, and with auto at left and side, it will center the element evenly horizontally.
due to .one margin top of 20px, it will make space outside of one element which resulted in pushing canvas 20px down.
So to fix it give padding of 1px to canvas class.
Now, canvas dimension becomes 502px 602px, to avoid dimension expansion,w e can set overflow property with a value of hidden, so that it wont push the entire element due to .one selector's margin property.
Add another div element inside canvas class, and give it a class of two.
use .two selector to select div element of class two and give it a width of 475px, height of 200px and background color of #8f0401
another rectangle will appear of dimension 475*200 px on bottom of div one, ofcourse div one and two will be separated with one margin-bottom which is 20px.
Now center the div element two with margin property set to auto.
Now add 3rd div inside canvas div and give it a class name of three.
use .three selector to select the div class three and set width to 91%, height to 28% and background color to #b20403.
third rectangle will appear beneath 2nd rectangle
now center the 3rd rectangle by giving margin proprty to auto in the .three class selector
it's helpful to have your margins push in one direction, as one pushed two down by 20px with margin, now do the same with two, as it already has margin on the top of one's bottom margin, need to set bottom margin of 20px, but we have alredy set margin to auto for .two, so to  make it work, edit margin property's value with 0(top) auto(right) 20px(bottom) auto(left)
Now according to the requrement, Rothko painting is blur, so we need to set the blurred color, to do that we have filter property, In .canvas class selector, give filter property the value of blur(2px).
Target .one and .two class selector and give it more blur by filter: blur(1px)
Increase blur of .three div element by 2px
Increase the area and soften edges of .one class selector by setting its box-shadow property with value of 0 0 3px 3px #efb762
here, box shadow has 0 horizontal offst, 0 vertical offset, 3px blur radius, 3px spread radius and color.
Now do the same with .two class selector.
Now do the same with .three class but this time give blur and spread radius of 5px instead of 3px.
the corners are still sharp which does not look like painting, so give it a border-radius of 9px in .one class selector.
Now do the same with .two class selector, but give the value of top left and bottom right border radius of 8px and top right and bottom left  with 10px by setting border-radius property to 8px 10px.
Now for .three div, give border-radius property the value of 30px top left, 25px top right, 60px bottom right and 12px bottom left, border-radius: 30px 25px 60px 12px;
Now to make it look like a painting, rotate a bit the rectangles in the canvas, we can do this by transform property and set the value of rotate(-0.6deg) to .one class to make it rotate by 0.6degree in counterclockwise direction
Now rotate .two by 0.4deg clockwise direction
Now rotate .three by 0.2 deg counter clockwise direction