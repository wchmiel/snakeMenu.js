# SnakeMenu
Simple jQuery plugin to make nice animated hover menu.

<br>
<h3>Static HTML</h3>
Put the script at the bottom of your markup right after jQuery:

<code> <script src="filespath/jquery-3.2.1.min.js"></script> </code> <br>
<code> <script src="filespath/snakeMenu-1.1.min.js"></script> </code>
  
<br>  
<h3>Usage</h3>

Wrap your menu items (div, a, img, span, li etc.) with a container element (div, ul etc.). Give them classes that you set
in the js snakeMenu cofig object:

        <ul class="snakeMenu">
          <li class="snakeMenuItem" data-menuitem="1"><a href="#home">Home</a></li>
          <li class="snakeMenuItem" data-menuitem="2"><a href="#about">About</a></li>
          <li class="snakeMenuItem" data-menuitem="3"><a href="#contact">Contact</a></li>
        </ul>
      
<br>
The same with the box element:   

        <div class="snakeBox">
          <div class="snakeBoxItem" data-boxitem="1">
            Content-1
          </div>
          <div class="snakeBoxItem" data-boxitem="2">
            Content-2
          </div>
          <div class="snakeBoxItem" data-boxitem="3">
            Content-3
          </div>
	    </div>

<br>
Call the plugin function and set the css classes for your elements or use default ones:

        $('.snakeMenu').snakeMenu({
          menuCont: '.snakeMenu',
          menuItem: '.snakeMenuItem',
          menuItemData: 'menuitem',
          boxCont: '.snakeBox',
          boxItem: '.snakeBoxItem',
          boxItemData: 'boxitem',
        });
	

<br>
<h3>Documentation</h3>

<h4>&bull; Classes</h4> 
&nbsp;&nbsp;&nbsp;With the following options you can change every class the way you want: <br><br>

1. <b>menuCont</b> <br>- Css class for the snakeMenu container:
<ul>
	<li>Type: Class / Id</li>
	<li>Default: '.snakeMenu'</li>
</ul>
<br>

2. <b>menuItem</b> <br>- Css class for the snakeMenu item:
<ul>
	<li>Type: Class</li>
	<li>Default: '.snakeMenuItem'</li>
</ul>
<br>

3. <b>menuItemData</b> <br>- Name of the data attribute for the snakeMenu items:
<ul>
	<li>Type: string</li>
	<li>Default: 'menuitem'</li>
</ul>
<br>

4. <b>boxCont</b> <br>- Css class for the snakeBox container:
<ul>
	<li>Type: Class / Id</li>
	<li>Default: '.snakeBox'</li>
</ul>
<br>

5. <b>boxItem</b> <br>- Css class for the snakeBox item:
<ul>
	<li>Type: Class</li>
	<li>Default: '.snakeBoxItem'</li>
</ul>
<br>

6. <b>boxItemData</b> <br>- Name of the data attribute for the snakeBox items:
<ul>
	<li>Type: string</li>
	<li>Default: 'boxitem'</li>
</ul>
<br>

7. <b>cssMenuItemActive</b> <br>- Css class to mark the active snakeMenu item (You have to define this class in css first):
<ul>
	<li>Type: string</li>
	<li>Default: 'snm-item-active' </li>
</ul>
<br>

8. <b>noActiveMenuItem</b> <br>- Css class that mark no active snakeMenu item (item is no active when appropriate boxItem is empty)
<ul>
	<li>Type: string</li>
	<li>Default: 'snakeItemNoActive' </li>
</ul>
<br>

<h4>&bull; Options</h4> 
&nbsp;&nbsp;&nbsp;List including all options for the snakeMenu plugin: <br><br>

1. <b>destroySnakeRes</b> <br>- Under this resolution the snakeMenu is diabled. (Then you can make your own menu for mobile resolutions)
<ul>
	<li>Type: number</li>
	<li>Default: 767 </li>
</ul>
<br>

2. <b>mouseDelay</b> <br>- This value defines delay beetwen a cursor enter the snakeMenu container and the snakeBox is open. This way your snakeBox won't be open when user is on snakeMenu item for less than define time. 
<ul>
	<li>Type: number</li>
	<li>Default: 300 </li>
</ul>
<br>

3. <b>boxOffsetTop</b> <br>- The value in pixels that define offset top beetwen the snakeMenu and the snakeBox (the snakeBox won't be closed when you hover that space area).
<ul>
	<li>Type: number</li>
	<li>Default: 0 </li>
</ul>
<br>

4. <b>boxOffsetBottom</b> <br>- The value in pixels that define offset bottom beetwen the snakeMenu and the snakeBox (the snakeBox won't be closed when you hover that space area).
<ul>
	<li>Type: number</li>
	<li>Default: 0 </li>
</ul>
<br>

5. <b>boxOffsetLeft</b> <br>- The value in pixels that define offset left beetwen the snakeMenu and the snakeBox (the snakeBox won't be closed when you hover that space area).
<ul>
	<li>Type: number</li>
	<li>Default: 0 </li>
</ul>
<br>

6. <b>boxOffsetRight</b> <br>- The value in pixels that define offset right beetwen the snakeMenu and the snakeBox (the snakeBox won't be closed when you hover that space area).
<ul>
	<li>Type: number</li>
	<li>Default: 0 </li>
</ul>
<br>

7. <b>animOpen</b> <br>- The function with your animation for the snakeBox. Invoked when the snakeBox is going to open.
<ul>
	<li>Type: function</li>
	<li>Default: jQuery fadeIn fn </li>
</ul>
<br>

8. <b>animOpen</b> <br>- The function with your animation for the snakeBox. Invoked when the snakeBox is going to close.
<ul>
	<li>Type: function</li>
	<li>Default: jQuery fadeOut fn </li>
</ul>
<br>
