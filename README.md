# The objective:
Welcome to my frogger demonstration videos and presentation page! The goal here is to recreate the classic game frogger with it's original rules onto a custom piece of hardware. The hardware is a DE1-SoC board, support a A9 dual ARM core processor. A "hard processor system" (HPS), allowing access to onboard FPGA peripherals and hardware memory addressing via virtual address linking. There will be three video demonstrations and presentation of my three week journey in replicating this game.

# The prototype 
Below is a short video depicting the moving hitbox prototypes and simpliest form of gameplay before adding more advanced algorithms for visual rendering. In essence the video rendering is made possibly by performing user level requests to the custom made kerenal driver for the VGA port. I developed the kernal driver for the VGA display port to be able to draw squares, lines and decisive pixels at specific locations and colors. The FPS in the top left corner is mislabelled and is actually counting how many frames has past, the game uses a double buffering system for pixel updating and erasing to be done. The true FPS is determined by how often the double buffer switches, the fastest time for the register flag to change is 1/60 seconds, i.e 60 FPS.
[![Video Title](https://img.youtube.com/vi/uN19iK474-Y/0.jpg)](https://www.youtube.com/shorts/uN19iK474-Y)


# With graphics
The video listed below will show more refined game mechanics with improved graphics thanks to Python script libraries like pillow to do image preprocessing to get pixel coordinates and color values. This mock up implements moving enemies (cars),object riding before reaching goal post and death animations. The presentation linked with this github post will elaborate more on the ideas, for code implmenetations please contact me.

<!-- [![Video Title](https://img.youtube.com/vi/9m5iKHtU3EM-Y/0.jpg)](https://www.youtube.com/watch?v=9m5iKHtU3EM) -->
[![Video Title](https://img.youtube.com/vi/9m5iKHtU3EM/0.jpg)](https://www.youtube.com/watch?v=9m5iKHtU3EM)

# Final product
This is the final product of my frogger game, I've implemented crocodile enemies, starting screen and a timer for added game pressure. Doing this project taught me how to plan technicals, simplify complex algorithms,realize hardware limitations and how to overcome them. If I were to improve this game more, I'd simplify unique variable calls and create more structures for better organization. Less usage of global variables to improve register look up speeds when stack frames are generated. Addiational features like a score board system with a simple CSV lookup can remember user scores from previous players. 

[![Video Title](https://img.youtube.com/vi/_BJbuDWveT0/0.jpg)](https://www.youtube.com/shorts/_BJbuDWveT0)


# Thanks for visiting!
Please do not reuse my material without permission, please contact me at calvinhuanli@gmail.com for inquires about this project. Please note the presentations have been modified to not include explict programming techniques for the DE1-SoC for copyright purposes. The presentations will go over programming concepts and technicals of user and kernal level relationships. More documentation on code can be provided upon request.