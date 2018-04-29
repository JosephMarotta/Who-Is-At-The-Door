# Who-s-at-the-Door
Amazon Alexa and Raspberry Pi project that allows a user to know who is exactly is knocking at their door using facial recognition

Checkout the project at https://www.hackster.io/gmelaub/alexa-who-s-at-the-door-d0f6b5

SENIOR DESIGN PROJECT - TEAM C48 
JOSEPH MAROTTA
VAHSTI MARIN
SPRING 2018

How we got it to work:

Start with fresh install of Rasbian OS. 
Format, and load NOOBS to mirco SD
Put SD in Pi, connected to monitor and keyboard
Select Rasbian OS when prompted and install
Plug pi into ethernet port

Run the following commands in the terminal
	terminal  : ‘sudo apt-get update’
terminal  : ‘sudo apt-get upgrade’ (might take a while)
terminal  : ‘sudo raspi-config’ (opens config GUI) 
	Select Interface options
	Enable Camera
	Finish and reboot

Test the camera
	terminal  : “raspistill -v -o test.jpg”
	Should have taken a picture

Install latest version of Node.js + NPM 
	“Curl -o- … command” 
	Todo: link online guide for this

Test versions using: ( look up latest arm71 nodejs )
node -v
npm -v	

	Confirm ‘node-modules’ folder exists in the /pi/ folder

(Optional: setup SSH) 

Download the Github File Repository (.zip) 
	Link: TODO
Extract the files to a known location within /pi/<some folder> 
(do not extract directly into /pi/ )

Setup Firebase and Karios API
	Firebase
	Karios API



Setup AWS Services
S3 storage bucket	
Lambda Solution

Set up Alexa Skill in Developer

Make necessary edits to the following files: (should be updated in forked github) 
	Firebase.js
	Database.js
	Index.js
	
	Confirm correct ‘node-modules’ folder is in /pi/

Start testing faces with Alexa Test

	Terminal : ‘node firebase.js’
	Run Alexa Test on Web Dev
	
	Watch event log on raspberry pi
	Watch AWS Lambda Event logs
	Watch Firebase Realtime Database Changes
	Test .json snippets with AWS Testing 

	Initial ‘gallery’ within Kairos API is “MyGallery” - firebase.js
