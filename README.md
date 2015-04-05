SourceRabbit GCode Sender
------
<p align="center">
<img src="https://raw.githubusercontent.com/nsiatras/sourcerabbit-gcode-sender/master/Images/SourceRabbit.png" alt="SourceRabbit.com"> 
</p>

SourceRabbit GCode Sender is a <b>GRBL</b> compatible, cross platform G-Code sender written in Java. It features a highly optimized and asynchronous (event-driven) UI and USB-to-Serial communication and can be also used on computers with small amount of RAM and CPU.

To run simply <b>download</b> and <b>unzip</b> the .zip file and <b>double click</b> the SourceRabbit-GCODE-Sender.jar file. On some platforms you will need to run an included start script.

Note for MAC users: You may need to create a "/var/lock" directory on OSX to fix a bug in the serial library. To do this open the Terminal application and run the following two commands: 
sudo mkdir /var/lock 
sudo chmod 777 /var/lock 

Technical details:
* Compatible only with <b>GRBL 0.9</b> and later versions
* Uses JSSC for serial communication
* Event-Driven UI and USB-to-Serial communication
* Developed with <b>NetBeans 8.0.2</b>
* To build you need to open the project in Netbeans and just... build.

Goals:
* Provide a fast, accurate and easy to use software
* Support all GRBL CNC router and milling machines
* Can be runned in computers with small amount of RAM and CPU.


Downloads
------

[1.0.2](https://github.com/nsiatras/sourcerabbit-gcode-sender/releases/download/1.0.2/SourceRabbit-GCode-Sender-1.0.2.zip) - Requires Java 7 or higher.


![Connect to your CNC!](https://github.com/nsiatras/sourcerabbit-gcode-sender/blob/master/Images/ConnectForm.png "Connect to your CNC!")

![CNC Control Form](https://github.com/nsiatras/sourcerabbit-gcode-sender/blob/master/Images/ControllForm.png "CNC Control Form")


Changelog
------
1.0.1 -> 1.0.2
* Fixed several UI bugs.
* Information Message box on GCode cycle finish.

1.0.0 -> 1.0.1
* Clicking the cancel button during GCode cycle stops the machine instantly.
* GCode cycle events implemented.
* GCode Sender can identify if the USB cable is plugged or not.
* Automatically skip blank lines and comments when sending a file.
