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
          <i class="snakeMenuItem" data-menuitem="1"><a href="#home">Home</a></li>
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

1. menuCont <br> - Css class for the snakeMenu container:
<ul>
	<li>Type: string</li>
	<li>Default: '.snakeMenu'</li>
</ul>
<hr>

2. menuItem <br> - Css class for the snakeMenu item:
<ul>
	<li>Type: string</li>
	<li>Default: '.snakeMenuItem'</li>
</ul>
<hr>

3. menuItemData <br> - Name of the data attribute for the snakeMenu items:
<ul>
	<li>Type: string</li>
	<li>Default: 'menuitem'</li>
</ul>
<hr>

4. boxCont <br> - Css class for the snakeBox container:
<ul>
	<li>Type: string</li>
	<li>Default: '.snakeBox'</li>
</ul>
<hr>

5. boxItem <br> - Css class for the snakeBox item:
<ul>
	<li>Type: string</li>
	<li>Default: '.snakeBoxItem'</li>
</ul>
<hr>

6. boxItemData <br> - Name of the data attribute for the snakeBox items:
<ul>
	<li>Type: string</li>
	<li>Default: 'boxitem'</li>
</ul>
<hr>

7. cssMenuItemActive <br> - Css class to mark the active snakeMenu item (You have to define this class in css first):
<ul>
	<li>Type: string</li>
	<li>Default: 'snm-item-active' </li>
</ul>
<hr>

8. noActiveMenuItem <br> - Css class that mark no active snakeMenu item (item is no active when appropriate boxItem is empty)
<ul>
	<li>Type: string</li>
	<li>Default: 'snakeItemNoActive' </li>
</ul>
<hr>
