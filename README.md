# Bus Ticketing System

## Purpose

This repository aims to provide a high level design for a Bus Ticketing system. It also contains a psuedo code for a Salesforce Evergreen function for a push notification.

### Table of Contents

- Axelerant_Bus_Trips_Viral : This document contains the High level solution document for the Bus Ticketing System.
- MobilePushNotification : This is a Salesforce DX Project which contains code for Salesforce Evergreen Mobile Push Notification.
- Diagrams : High quality diagrams of the images used in the document. It contains the System Architecture, Data Model and Use Case diagrams

#### Notes

1. I have created a SF DX project from scratch and hence most of the folders will be empty since the ask was only for an Evergreen function.
2. The Evergreen function can be found at \MobilePushNotification\force-app\main\default\functions\PushMobile
3. Since Salesforce Evergreen is still in beta mode, the function is a not tested high level code that would potentially work.
4. Steps used to create an Evergreen function are as below:
	- Create a new SF DX project using: 
		```
		$ sfdx force:project:create --projectname mywork
		```
	- Install the beta evergreen package using:
		```
		$ sfdx plugins:install @salesforce/plugin-evergreen
		```
	- Move to the directory : 
		```
		cd \force-app\main\default
		```
	- Create a new SF Evergreen function using:
		```
		$ sfdx evergreen:function:create MyFunction --language=javascript
		```
