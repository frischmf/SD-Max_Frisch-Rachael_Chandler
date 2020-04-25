# Final Report

## Table of Contents
1. [Project Description](#project-description)
2. [User Interface Specification](#user-interface-specification)
3. [Test Plan](#test-plan)
4. [User Manual](#user-manual)
5. [Spring Final PPT Presentation](#spring-final-ppt-presentation)
6. [Final Expo Poster](#final-expo-poster)
7. [Assessments](#assessments)
    * [Initial Self-Assessments](#initial-self-assessments)
    * [Final Self-Assessments](#final-self-assessments)
8. [Summary of Hours & Justification](#summary-of-hours-and-justification)
9. [Summary of Expenses](#summary-of-expenses)

***

## Project Description

Plants can be difficult to take care of - they require consistent attention, different species need different care, and unless you are familiar with plants you may not know what it is that a plant needs to be healthy or what is lacking in the care you provide. 

We seek to create a holistic solution to this problem, by creating an interactive system that supplements the caretaking process and provides helpful insight to improve the health of your plant. 
We aim to monitor plant health and provide the plant-owner with relevant caretaking information. This will be accomplished using a Raspberry Pi to measure different metrics related to plant health (exposure to light, rhizosphere moisture level, pH, and relative humidity), and then will be analyzed to provide the user with helpful feedback regarding plant health and advice for future care.

***

## User Interface Specification

### Sign In

The Sign-In screen is the first interface the user experiences, from here they have the ability to sign in with a pre-existing account or to create a new one.

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/SignIn.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/SignIn.png" alt="Sign In" width="180" height="360" /></a>

### Create Account

If deciding to create an account, all that is required is to enter your name, email, and password. This then generates a user token and allows you to automatically sign in upon opening the application again.

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/CreateAccount.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/CreateAccount.png" alt="Create Account" width="180" height="360" /></a>

### Plant List

This is the central hub, after signing into the application this is the interface that the user is most often presented with. It was created with the intent of easily showing the overall status of your garden's individual plants at a glance. Upon selecting an individual plant you are brought to that plant's overview where you can look into more detailed and current information.

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantList.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantList.png" alt="Plant List" width="180" height="360" /></a>

### Plant Overview

The overview is designed to present current plant factors gathered, and to quickly provide feedback as to which ones could use some immediate work. Factors bolded in red are in "danger" and need attention. If the user is seeking more detailed information as to bringing those danger factors into a safe range, they can hit the hyperlink "Plant needs some attention" to bring up their "Plant Tips".

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantOverview.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantOverview.png" alt="Plant Overview" width="180" height="360" /></a>

### Plant Tips

Plant Tips are personalized to the constraints of the particular plant-type and its current needs. It provides instant feedback that clues the user into what we believe is a safe range for the selected plant.

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantTips.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/PlantTips.png" alt="Plant Tips" width="180" height="360" /></a>

### Historical Averages

Historical Averages are presented to allow the user to see the progress they've made and to have a means of keeping track of their plant's health over a period of time. This screen is accessed from the bottom navigation bar by selecting "Logs".

   <a href="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/HistoricalAverages.png" target="_blank"><img src="https://raw.githubusercontent.com/frischmf/SD-Max_Frisch-Rachael_Chandler/master/Senior%20Design/Final%20Report/res/HistoricalAverages.png" alt="Historical Logs" width="180" height="360" /></a>


***

## Test Plan

[Test Plan](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/TestPlan.md)

***

## User Manual

[User Documentation](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/User%20Documentation.md)

***

## Spring Final PPT Presentation

* [Final Presentation](https://youtu.be/ASxNq7-KsSI)
    
    <a href="http://www.youtube.com/watch?feature=player_embedded&v=ASxNq7-KsSI" target="_blank"><img src="http://img.youtube.com/vi/ASxNq7-KsSI/0.jpg" alt="Final Presentation" width="240" height="180" /></a>

* [Demo Video](https://youtu.be/G5G5Bd6gEag)

    <a href="http://www.youtube.com/watch?feature=player_embedded&v=G5G5Bd6gEag" target="_blank"><img src="http://img.youtube.com/vi/G5G5Bd6gEag/0.jpg" alt="Demo Video" width="240" height="180" /></a>

***

## Final Expo Poster

[Poster](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/Poster/Senior%20Design%20Poster_Final.pdf)

***

## Assessments

### Initial Self-Assessments

[Max's Initial Self-Assessment](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/Fall%20Assignments/Assignment%203/Assignment%203%20-%20Max%20Frisch.md)

[Rachael's Initial Self-Assessment](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/Fall%20Assignments/Assignment%203/Assigment%203%20-%20Rachael%20Chandler.md)

### Final Self-Assessments

[Max's Final Self-Assessment](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/Final%20Self-Assessments/SelfAssessment_Max.md)

[Rachael's Final Self-Assessment](https://github.com/frischmf/SD-Max_Frisch-Rachael_Chandler/blob/master/Senior%20Design/Final%20Self-Assessments/SelfAssessment_Rachael.md)

***

## Summary of Hours and Justification

[Summary of Hours - Spring Semester](https://docs.google.com/spreadsheets/d/1oC78x76Ll7wg6k66jJxOG4p9fTJtGcVxjtpfKQ69jag/edit?usp=sharing)

***

## Summary of Expenses

### Hardware Costs
* Raspberry Pi ~ $40
* Soil Moisture Sensor ~ $10 - $15

* Humidity Sensor ~ $10
* Light Intensity Sensor ~ $9
* Analog to Digital Converter ~ $15
* SD Card, Power Supply ~ $25
* Wiring / Breadboards ~ $16

### Research Supplies
* Pots, Plants, Soil... ~ $40

**Actual Cost: ~$170**




