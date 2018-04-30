![alt text](https://github.com/CSUGameOfThreads/RaspberryPi/blob/master/static/img/abblogo.png "Andre Brandon Brian")
# Raspberry Pi Security Camera
Home Surveillance with Raspberry with a total of 342 lines of Python Code and 192 lines of HTML.
For technical details check the realted files below.

## static 
  - img
    - ```abblogo.png```
    - ```csulogo.png```
    - ```got.png```
  - styles
    - ```style.css```
***

## templates 
- #### ```index.html```
  - Landing page with a basic html code supported by jQuery in order to send on/off ajax requests to our server and to update the system status.
- #### ```credits.html```
  - Extra page with project credits and copyrights
***

## ```conf.json```
  - Determines which email the pictures will be sent to
  - Sizes the images taken from the Raspberry Pi before sending them over email
***

## ```flaskapp.py```
  - Loads the website from the templates folder
  - Starts and stops the watching code and returns output into terminal
  - The web server framework.
***

## ```pi_surveillance.py```
  - Checks to see if the Dropbox should be used
  - Initialize the camera and grab a reference to the raw camera capture
  - Capture frames from the camera
  - Check to see if the frames should be displayed to screen
***

## ```utils.py```
  - Using the defined mail address on gmail, it send a alert mail with attached images
  - Taken frames are kept in /tmp folder with concecutive numbering. 
  - Includes the email credentials
***

## ```utils.pyc```
  - Extra file from the utils.py
***

![Alt Text](http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif)
