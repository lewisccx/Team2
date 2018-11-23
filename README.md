# 2x01Project
VR Safe Riding Project


# VR-Riding
VR-Riding is a virtual reality (VR) software application that allows cyclists and personal mobility device (PMD) users to practice safe riding on Singapore roads, walkways and shared paths. VR-riding also allows the users to have a free range of motion within the area and give them the feelings of immersion within the virtual environment, thus providing a pleasant and intuitive experience. Ultimately, the aim of VR-riding is to educate users on the safety aspect of commuting by cycling or with their PMD’s in Singapore.

This file shall describe the information of the VR-Riding application, and guides users to install and use the application.

## VR-Riding Functional Requirements
This section describes the core functionalities of VR-Riding and what it must be able to perform and deliver. After gathering requirements from the client, it is agreed that VR-Riding shall be able to:
1. Display instructions and descriptions in common languages.
2. Validate users based on authority, namely the Player and SCTF Admin roles.
3. Educate Players on the appropriate actions to do when commuting using bicycles or PMDs.
4. Work across most VR devices.
5. Display virtual environment as close to real environment, such as Singapore roads and Park Connector Networks (PCN) as possible.
6. Allow SCTF Adminstor to edit the virtual environment, such as changing the average number of vehicles on the road, the average number of pedestrians on the street and the background environment.
7. Provide users the correct safety information when they do dangerous actions in the game.
8. Provide 5 different 10-minute-long levels of simulated riding in the virtual environment. 
    The information of the levels are:
	1. In each level, users are by default travelling forward and can choose to stop by pressing the brake button(e.g. to stop 		during red light.). 
	2. In levels 4 and 5, users can also choose to turn left and right to avoid pedestrians.
	3. Questions pertaining to safe riding will also be displayed to the users throughout the game.
	4. Level 1: Players are only allowed to travel forward and there are only traffic lights in the game.
	5. Level 2: Players are only allowed to travel forward and there are cars and traffic lights in the game.
	6. Level 3: Players are only allowed to travel forward and there are cars, zebra crossings and traffic lights in the game.
	7. Level 4: Players can travel forward and make left and right turns. There are cars, zebra crossings,pedestrians and traffic 	            lights in the game.
	8. Level 5: Players will be placed in a night version of the game and they can travel forward and make left and right turns. 	            There are cars, zebra crossings, pedestrians and traffic lights in the game.
9. Provide analytical data on the performance of the Player (e.g. Player tend to ride on right side of the road)

## VR-Riding Non-Functional Requirements
1. Product constraints: Device must be able to support VR and users must know how to operate a VR application. 
2. Organizational Constraints: Organization is only able to invest in certain VR headsets and not give the full experience. 
3. External constraints: Environment and knowledge in VR application.   
4. Product must be user friendly and easy to understand so that users are able to use it intuitively without much guidance.
5. System shall ensure that users are able to understand and finish the levels.
6. System shall give encouragement when users answer a question correctly.

## Setup 

### Project URL
* [Project Link: Google Drive](https://drive.google.com/open?id=1HVzAYGdR2tUlPMDpsFwt39b-0ySC7_s4)

### Dependencies

* [*GoogleVR*](https://github.com/googlevr/gvr-unity-sdk) - For character control, event control & trigger
* [*Android 4.4 (API level 19) and Above - KitKat and above*](https://developer.android.com/studio/) - Android SDK

### Installation
#### Windows
1. Download Unity Hub and run 
2. Install Unity3D from Unity Hub
3. Run Unity Hub > Open > Located and select “VRsafeRiding” folder
4. Click on "Play" button in Unity3D
5. Hold down Ctl + Alt key and left click to control your movement and rotation in the game  

#### Android
1. Enable “Installation of Non-Official Apps” in your android mobile phone (open Settings > Advanced Settings > Security > Enable 	    “Unknown Sources”)
2. Transfer VRsafeRiding_1.0.apk file into your phone storage
3. Install VRsafeRiding_1.0.apk file 

## Walkthrough

### SCTF Admin Manual
* Select "SCTF Admin" option role
  * To view player analytics (last played game)
    1. Select "View Analytics" in the Admin Panel
  * To set game setting 
    1. Select "Game Setting" in the Admin Panel
    2. Select "Game Level" (1 - 5) 
    3. Select desired number of vehicles, pedestrians, traffic lights (from 0 to 30) and environment for the chosen level.
  
### Player Manual
1. Select "Player" option
2. Select a "Level" (1-5) you desire (level details will be displayed on the screen)
3. Select a "Vehicle" you desire
4. Select "Play" option to play the game
5. Explore the map by:

5a. For Android: press on the screen to move forward and face the direction to control the direction you want to turn.
5b. For UnityHub on Windows: Hold down Ctl + Alt key and left click to control your movement and rotation in the game.  
6. Answer questions and practise safe riding with the game. Have fun with the game!

### Developer Manual
1. All the elements displayed (included vehicle, buildings, pedestrian and etc) in the game are located in the “VRsafeRiding ” > “Assets” folder
2. All the backend C# scripts are located in the “VRsafeRiding ” > “Assets” > “Scripts” folder

### Game Rules
 1. Locate and answer the quiz questions in the game around the map
 2. Avoid hitting pedestrians as well as getiing hit by vehicle and pedestrian 
    in the game
 3. Each question act as a checkpoint (save game progress) in the game 
 4. To restart the game, click on the restart menu located the at the start of the map.

## Demo
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/oi3-u31Q5kc/maxresdefault.jpg)](https://www.youtube.com/watch?v=oi3-u31Q5kc)  
*Youtube Link: https://youtu.be/v=oi3-u31Q5kc*

## Contributors

*  _Cao Chenxing - Quiz logic_
*  _Han Yu Fong Joseph - Scene Change logic_
*  _Jeremy Tan Teng Tat - Game Menu Logic_
*  _Lim Jia Hui Alissa - Save User State logic_
*  _Lim Yoong Jin - Night Mode Logic_
*  _Ng Zhi Yuan - Traffic Light Logic_


## Errors and bugs
   1. Player is not facing the quiz question when he changes scene
   2. Player's screen camera and his bicyle is able tilt up/down 90 degree at the same time
   
## Limitations
   1. There are no traffic rules implemented in the game, but you encouraged to adhere to them to score more points!
   2. VR-riding currently only supports android mobile
   3. Player's Phone has to be in left screen orientation 

## Feedback
   1. To implement a Health Point system 
      * Player lose a portion of his health whenever he hitted by vehicle and eventually lose the game if his health runs out
   2. To implement Play-Time Limit system
      * If player unable to finish the game with time limit given, he loses the game

## Frequently Asked Questions (FAQ) 

Q: What platforms are supported?

``` 
A: Devices running Android KitKat and above, and Windows with UnityHub installed

```
Q: How does a player start the game?
```
A:  1. Select "Player" option
    2. Select a "Level" (1-5)
    3. Select a "Vehicle"
    4. Select "Play" option
```

Q: I have a new bug or feedback to report. Who do I contact?
```
A: Please contact the development team at 1700208@sit.singaporetech.edu.sg.
```

Q: Why was this game created?
```
A: This game was created to help allow cyclists and personal mobility device (PMD) users to practice safe riding on Singapore roads, walkways and shared paths. 
It is hoped that with the game, users can be educated on the safety aspect of commuting by cycling or with their PMD’s in Singapore. 
The game achieves this by asking meaningful safe riding-related questions and giving praises or feedback to users when required.
```

## Copyright and Attribution

Copyright (c) 2018 2x01Team2. Released under the [MIT License](https://github.com/lewisccx/Team2/blob/master/LICENSE.MD).
