# Why Omron Sucks
The ugly sides of Omron:

1. You can't replace a function block with an identical one (such as replacing _CP2E030_SendModRTU_F03_P1 with _CP2E030_SendModRTU_F03_P1EX in order to change the target serial port) without deleting all function parameters. You have to delete everything and write the function arguments from start. 

2. Their programming software is sold and sold with a high price. Why? Why should I pay money to program/configure a device that I already bought? Do you pay for modem software that you bought from a store or do you simply type 192.168.1.1 to configure the device via the web interface? They are the same. 

3. UI problems: Dialogs that you can neither resize nor read the dropdown contents: 

    ![image](https://user-images.githubusercontent.com/6639874/181508557-e8fdd219-6d88-40c1-b01d-18d6aa9b7c3f.png)


# Documentation

1. Their documentation is way much longer than it should be. WAY MUCH LONGER. They are full of unnecessary images and paintings. Reading the documents is almost impossible in practical situations.

2. Documentations are organized carelessly. Example: You should write down the data address range that the Modbus TCP Server library handler writes the incoming data into at the start of your document. This is the first thing developer needs. They did write this information at page 15 in a 26-page-document. 
