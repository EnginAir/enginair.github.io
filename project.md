---
layout: page
title: Project
sidebar_link: true
---

## Problem
During a flight, the Engine Control Unit (ECU) saves trending and maintenance data which is reported to the mechanics and engineers via a hardware diagnostic report. Proper upkeep is important to prevent maintenance delays and keeps the engine functioning properly to ensure a safe flight.

![Problem 1]({{ site.baseurl }}/img/prob1.png)

Currently, Honeywell engine operators are required to download and send engine diagnostic data reports once a month. This process requires:
1. a manual port connection using a USB device and a cable,
2. transferring a file to a USB drive, and
3. sending the file via email.
This process is tedious and collects a small data set containing basic maintenance information. Because this process occurs once a month, it can result in infrequent data collections and missed maintenance opportunities.

![Problem 2]({{ site.baseurl }}/img/prob2.png)

To better this process and collect flight data more frequently, Honeywell is currently developing a connected engine product called the Connected Engine Data Access System (CEDAS). CEDAS allows engines to autonomously upload engine data wirelessly to a cloud. The CEDAS is hosted on an embedded computer located in the aircraft along with a WiFi antenna. If the WiFi connection is spotty or nonexistent at a certain location, the diagnostics may not send. When this happens and the data upload is not on schedule, it is difficult to determine the status of the aircraft; whether it is grounded, inflight, or if there is a potential problem with the engine. 

The initial concept for this project was provided by our sponsor and can be found [here](https://www.cefns.nau.edu/~edo/Classes/CS_Capstone/Projects/F19/Mitchell-WiFi-Signal-Location.pdf).

## Solution
To solve our client’s problem, our team has come up with the Connected Engine Upload Status System (CEUSS). Two primary goals of this system are: 1) provide airplane operators a way to know where to park their aircraft for the highest chance of upload success and 2) provide engineers a way to be notified and help visualize where and when potential problems occur. CUESS is composed of two main components: the server-side backend software which is primarily responsible for the data import and execution of database correlations, and the administrative front end web panel which is primarily used as a graphical interface to display notifications and LON/LAT locations.
A high-level workflow of our solution is outlined below:
![Solution Workflow]({{ site.baseurl }}/img/solution.png)

## Requirements
To implement our solution, we have outlined five high-level requirements:
- We need to determine which public flight database to mine 
- We need to create a server-based program to take in information from flight databases & correlate data
- We need to build a website for the client
- We need to build a database to store information
- We need a way to graphically illustrate the various metrics (i.e. Wi-Fi strentgh, flight paths, etc.)

We describe our lower-level requirements in the form of user stories to explain the functionality for the different types of end-users: engine technicians and airplane operators. Engine technicians are more interested in knowing the technical aspects of the aircraft upload process (i.e., upload failure explanations, landing locations, status of upload entry, etc.) while the aircraft operators (i.e. pilots) are more concerned with the big picture like where to park the aircraft to ensure a successful upload.

The eight user stories are listed below:

As an engine technician, I want to be able to:
- view all aircraft landing locations, every 24 hours.
- visualize all flights that are currently in progress.
- simulate various locations and their corresponding WiFi configuration.
- know the status of each landing/upload entry.
- visualize the status of each upload entry
- run a report to determine the cause of a failed upload.

As an aircraft pilot/operator, I want to be able to:
- visualize locations on where to park the aircraft for an upload success.
- simulate locations and their WiFi strength.

## Technologies
To complete the high-level requiremments, our team is reserached different technologies that can be used to complete of our project.

Chosen Technologies:
- Public Flight Database: ADSB Exchange 
- Server Application: Java
- Front End Web Application: NGINX
- Back End Web Application: NodeJS
- Database: MongoDB
- Graphical Illustration Application: OpenStreetMap

Last update: 12/4/2019
