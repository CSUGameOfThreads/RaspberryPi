# RaspiSecurity
Home Surveillance with Raspberry with only ~100 lines of Python Code and ~150 lines of HTML.
For technical details check the realted files below.

# templates 
- ### ```index.html```
- Landing page with a basic html code supported by jQuery in order to send on/off ajax requests to our server and to update the system status.
- ### ```credits.html```
- Extra page with project credits and copyrights
- ### static
***
- Has the Fonts, img and styles frolder for the HTML files
***

## ```conf.json```
- Determines which email the pictures will be sent to
- Sizes the images taken from the Raspberry Pi before sending them over email

## ```flaskapp.py```
- Loads the website from the templates folder
- Starts and stops the watching code and returns output into terminal
- The web server framework.

## ```pi_surveillance.py```
- Checks to see if the Dropbox should be used
- Initialize the camera and grab a reference to the raw camera capture
- Capture frames from the camera
- Check to see if the frames should be displayed to screen

## ```utils.py```
- Using the defined mail address on gmail, it send a alert mail with attached images
- Taken frames are kept in /tmp folder with concecutive numbering. 
- Includes the email credentials

## ```utils.pyc```
- Extra file from the utils.py
