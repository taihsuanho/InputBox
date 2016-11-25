# InputBox
A text input bar editor for pygame

Function
--------
InputBox(rect, **args)

Arguments
---------
rect: create the bar editor in the region defined by rect.

Keyword arguments
-----------------
font: font of the input text.  
text: text in the input bar initially.  
bk_image: background image of the text input bar.  
bk_color: background color of the text input bar, ignored when bk_image is specified.  
bd_color: border color, no border if this keyword is missing or None.  
text_color: color of the input text. White color if this keyword is missing.  

Return value
------------
Return (input text, flag), where flag can be True, False, or None when pressing ENTER,  
ESC, or receiving QUIT event.  

Comments
--------
The input bar is transparent if both bk_image and bk_color are not specified or None.  
There is a game loop inside this function, and all events will be ignore except for  
the key events and QUIT, which will be put back to the event queue and exit the game  
loop.  
