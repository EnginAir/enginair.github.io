---
layout: page
title: Project
sidebar_link: true
---

## Problem
A flight delay is something no passenger or flight crew wants to experience – yet we’ve all been there.  Mechanical delays routinely cause aircrafts to be grounded minutes before departure.  This wastes money, time, and causes for an unpleasant flight experience.  In order to prevent these unwanted delays, fight data via diagnostic reports are reviewed by engineers and mechanics.  Currently, Honeywell engine operators gather this data manually, with a manual port connection and a USB.  This tedious process occurs only once a month, leading to infrequent data collections and missed maintenance opportunities. 
 
To better this process and collect flight data more frequently, Honeywell is currently developing a connected engine product called CEDAS (Connected Engine Data Access System). CEDAS is an autonomous system that allows engine data diagnostics to be uploaded wirelessly to the cloud.  The problem with this is that diagnostics may not send if the Wi-Fi connection is spotty or nonexistent at a certain location.  When this occurs and a data upload is not on schedule, it is difficult to determine whether the aircraft is grounded, in flight, or if there is a problem with the engine. 

The initial concept for this project was provided by our sponsor and can be found [here](https://www.cefns.nau.edu/~edo/Classes/CS_Capstone/Projects/F19/Mitchell-WiFi-Signal-Location.pdf).

## Solution
Our solution consists of three subparts:
- Landing Monitor: collects landing location data (latitude/longitude) where indivudal engine startup/shutdown occurs
- WiFi Configuration Manager: maps specific longitude/latitude points on a map corresponding to a specific aircraft upload point
- Customer Connection Module (Sophisticated Web Portal): grahphically illustrates flight paths, landing data, and Wi-Fi strength at specific locations

## Requirements
To implements our solution, we have outlined five high-level requirements:
- We need to determine which public flight database to mine 
- We need to create a server-based program to take in information from flight databases & correlate data
- We need to build a website for the client
- We need to build a database to store information
- We need a way to graphically illustrate the various metrics (i.e. Wi-Fi strentgh, flight paths, etc.)

## Technologies
To complete the high-level requiremments, our team is reserached different technologies that can be used to complete of our project. Any documentation that is released for our technology feasability will be made available on our “Document Archive” page of this website.      

Chosen Technologies:
- Public Flight Database: ADSB Exchange 
- Server Application: Java
- Front End Web Application: NGINX
- Back End Web Application: NodeJS
- Database: MongoDB
- Graphical Illustration Application: Google Maps

Last update: 12/4/2019
