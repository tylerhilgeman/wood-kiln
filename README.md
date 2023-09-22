# Wood Kiln Startup Guide

## Purpose:
To serve as a guide to download, edit, and upload this code to your Arduino powered wood kiln.

## 1. Download the Arduino IDE
- Download the Arduino IDE to your computer from [this link](https://www.arduino.cc/en/software).

## 2. Download the code file
- Clone this project or download the file you want to use. The included files are in the `code` folder.
  - `mainKiln.ino` is the code that is currently on the device, pieces of the code has comments that give a bit more context to the decision making tree involved.
  - `warmer.ino` is another program that I used during the winter that keeps the kiln at a constant temperature in colder weather. I stored paint and chemicals in here at 50°F instead of letting it freeze in the barn this past winter. Change the `setTemp` variable to the temperature you want the kiln to maintain. Follow the steps below to update the kiln.
- Open it in the Arduino IDE.

## 3. Making changes to the code file
- You can edit the code at any time in the IDE.
- Arduino programs are written in C++, so if you make any major changes make sure you are following C++ syntax.
- [Click here for the Arduino reference guide.](https://www.arduino.cc/reference/en/)
- [Click here for a reference to C++.](https://www.w3schools.com/cpp/)
- Save your changes when you are done. You can do this in a new file if you want to keep different versions.

## 4. Uploading code to the Arduino
- I included a yellow USB cable with the kiln. Plug this into your computer.
- Make sure the main power to the kiln is disconnected. The Arduino will be powered by your computer while its plugged in, but the lights, fan, and dehumidifier won't turn on.
- You may need to select the appropriate port that your Arduino is connected to.
  - Visit "Tools" in the top menubar and confirm that your board reads "Arduino Uno."
  - Your port may not default to the port that the Arduino is connected to. Hovering over "Ports," again in the "Tools" menu, will show you the ports. The correct one should say Arduino. Select it.
    ![SelectBoardAndPort.png](https://github.com/tylerhilgeman/wood-kiln/blob/3c7a913988ea65933d55199f67eab5daac0c13ac/SelectBoardAndPort.png)
- Click the "Verify" button (Checkmark) in the top left of the screen to compile the code and confirm you don't have any compile time errors. This is the red square in the image below.
- If you have no errors, click the "Upload" button (Arrow) next to the "Verify" button to upload the code to your Arduino. This is the orange square in the image below. You will see a progress indicator and should be able to see the Arduino go through its setup process on the screen if the upload is successful.
  ![ArduinoIDEUploadAndVerifyButtons.png](https://github.com/tylerhilgeman/wood-kiln/blob/a19c5a7a494155eb2305f690b144db7e5d5d0fa6/ArduinoIDEUploadAndVerifyButtons.png)
- After the code is uploaded, plug the kiln's power in again.

## 5. Software Troublshooting Tips
- Opening the serial monitor in the IDE while your computer is connected will show more values that are commented into the code. Here, you can troubleshoot.
- The board has a small white reset button that you can press while the Arduino is on, which will keep the code but will restart the program.
  


