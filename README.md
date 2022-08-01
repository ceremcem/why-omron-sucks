# Why Omron Sucks
The ugly sides of Omron:

# CX Programmer

1. You can't replace a function block with an identical one (such as replacing _CP2E030_SendModRTU_F03_P1 with _CP2E030_SendModRTU_F03_P1EX in order to change the target serial port) without deleting all function parameters. You have to delete everything and write the function arguments from start. 

2. Their programming software is sold and sold with a high price. Why? Why should I pay money to program/configure a device that I already bought? Do you pay for modem software that you bought from a store or do you simply type 192.168.1.1 to configure the device via the web interface? They are the same. 

3. UI problems: Dialogs that you can neither resize nor read the dropdown contents: 

    ![image](https://user-images.githubusercontent.com/6639874/181508557-e8fdd219-6d88-40c1-b01d-18d6aa9b7c3f.png)

4. You need to turn off and then turn on the PLC in order to the Settings take effect. You have to know (or somewhat guess) that, there is no warning. 


# Documentation

1. Their documentation is way much longer than it should be. WAY MUCH LONGER. They are full of unnecessary images and paintings. Reading the documents is almost impossible in practical situations.

2. Documentations are organized carelessly. Example: You should write down the data address range that the Modbus TCP Server library handler writes the incoming data into at the start of your document. This is the first thing developer needs. They did write this information at page 15 in a 21-page-document. 
![image](https://user-images.githubusercontent.com/6639874/181598207-a0306175-6378-4914-8ae7-ba5013faf430.png)

3. Data areas mentioned in the documentation as, eg., `D100` and you have to type `D100` in CX Programmer. However, input registers are mentioned within the documentation as, eg., `IR 002`, but you have to type `2` as the data address in CX Programmer. You have to know that. 

4. Documentation is written in a poor English, which leads confusions. 

5. Documentation does not have to cover all the error codes:

![image](https://user-images.githubusercontent.com/6639874/182104078-9ede2d31-1c5d-4b43-b98c-e6c078ca570a.png)

> Note that they have Error code of `008F Hex`, which means `Other Error`. You have to guess what this error might be. They trust you. 

# Technical Support

1. Omron support engineers might only have some ideas about popular questions. For example, they have no idea about if their own RS-232 port works with their own Modbus RTU stack. 
