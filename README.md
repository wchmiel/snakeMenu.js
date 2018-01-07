# SnakeMenu
Simple jQuery plugin to make nice animated hover menu.


# Static HTML
Put the script at the bottom of your markup right after jQuery:

<code> <script src="filespath/jquery-3.2.1.min.js"></script> </code> <br>
<code> <script src="filespath/snakeMenu-1.1.min.js"></script> </code>
  
# Usage

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
