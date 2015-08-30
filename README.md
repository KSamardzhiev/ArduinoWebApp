# Arduino Web App

*This project make possible to remotely enable/disable a LED on Arduino using PHP and Processing*

The idea of the project is very simple, and could easily be altered to enable remote control of relays or other different types of outputs. The great thing about using a web interface is that it is cross-platform and pretty much enables you to also control your Arduino using most devices with web browsing capabilities, such as smartphones and tablets.

In the project I used:

    - An Arduino board with an internal LED (usually on pin 13) or a separate LED
    - A webhosting service with PHP support
    - The Arduino IDE
    - The Processing IDE

The function of the web interface is to give the user the choice to either switch the LED on or off. When either one of them is clicked, the command is written to a .txt-file as a 1 (ON) or 0 (OFF) value.
The interface consists of three files; a HTML front-end, a PHP document, and a .txt-file for storing values.

The part that ties all files and logic together is Processing sketch. It reads the stored values in the .txt file and talk to Arduino through particular port. 

This project is written with the help of this post: [How to remotely enable/disable a LED on your Arduino using PHP and Processing](http://projects.sindrelindstad.com/how-to-led-arduino-php-proc/)
