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

Plant Parenthood is an attempt to facilitate and modernize the at-home plant care experience. Our goal is to provide education and assistance for at-home plant care in a way that is accessible, affordable, and attractive through the use of effective metrics, valuable user feedback, and an aesthetically pleasing mobile application.

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

#### FAQ

* Where can I get one of these fancy Plant Parenthood hubs? Sign me up!

    These hubs are still in development, and were produced for the purpose of our Senior Design project. Other than the demo hub, none other exist... for now.

* I only receive one notification a day but would like to get more. How can I make that happen?

    While developing this solution we didn't want to overwhelm you with multiple notifications a day - we wanted the care taking experience to feel enjoyable, not as if you were being nagged. We may in the future implement preferences for notifications, as well as preferred constraints for a particular plant, rather than just determining what we think is healthy based on the type of plant it is.

* Plant Parenthood says my apartment is 165 degrees Fahrenheit and -40% humid... what's up with that?

    To keep Plant Parenthood affordable we've done our best to compromise between affordable sensors and effective data gathering. This is a rare problem, but it does happen... and it's always fixed by a good whack to the hub!


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

#### Max's Final Self-Assessment

I contributed the majority of the software and hardware implementation of the Plant Parenthood project. This includes putting together the Raspberry Pi, installation into the plant, and laying the architecture for the solution – I created and deployed the database, API, Pi, and Android client and ensured that each endpoint was able to communicate with each-other. I certainly applied and built upon the foundation of the initial assessment from the Fall, but I feel that much of my learning came from the unforeseen difficulties and challenges that came from creating this project from the ground up.

More specifically I learned how to create a service (that begins on startup) on a Raspberry Pi, able to read sensor data and communicate that data with a server utilizing gRPC. That server (the API) functions as the control layer that communicates with the Azure SQL Database through Entity Framework, and also feeds data directly to the Android client written in primarily Kotlin. I feel that I’ve become far more competent in producing functional project architecture – the most difficult part was just getting everything set up. Once we had the connection wired and gRPC was functioning as expected the rest followed from prior experience within the Computer Science curriculum. I also feel that I’ve grown in competency programming in multiple languages (C#, Python, Kotlin, Java), I feel that I’ve significantly grown in my understanding of real data retrieval and the hardware aspect of computer engineering, and I have a much better understanding of the client / server relationship.

To be honest, Covid-19 was a major obstacle. There were many parts we weren’t aware that we needed until we needed them (Analog to Digital Converter, additional wiring, breadboards, soldering), and at that point shipping moved from 2 days to 3 weeks and our ability to shop freely was significantly inhibited. We found what we needed, but it was certainly an unforeseen difficulty.

#### Rachael's Final Self-Assessment

A big part of my role for this project was project planning and management. I created schedules and made sure we stayed on track, researched all the equipment we would need and created our expense report, and kept track of meetings that we had. I also did a lot of work for the two presentations that we created, contributing content to the power points and narration. I worked with our advisor to create a scope for our project, and then build ideas for how our project could be utilized in the future (such as increasing the scale and adding commercial applications).

I learned a lot about project management. I had never really taken on a project of this scope before, so my past projects didn’t have as much of a need for project management. I was not as involved with the coding of our project, largely because of the quarantine that went into effect half way through the semester, but there was still a lot to contribute as far as working on the poster and content of the project, and making it easy to understand from an outside view. I feel that our project turned out quite well in light of the circumstances of this semester. One of the largest obstacles to me was the quarantine. I traveled during spring break, so when I returned, I had to self-quarantine for 2 weeks. After that, the entire state was quarantined, and my partner and I could no longer meet in person. Since he had all the hardware, there wasn’t a whole lot I could do to help with the building and testing of our project. However, I feel that my contribution to our project was still significant, especially in our presentation tools.

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




