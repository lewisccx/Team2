# 2101Project
VR Safe Riding Project


# VR Riding
VR-riding is a virtual reality (VR) software application that allows cyclists and personal mobility device (PMD) users to practice safe riding on Singapore roads, walkways and shared paths. VR-riding also allows the users to have a free range of motion within the area and give them the feelings of immersion within the virtual environment, thus providing a pleasant and intuitive experience. Ultimately, the aim of VR-riding is to educate users on the safety aspect of commuting by cycling or with their PMD’s in Singapore.

## VR Riding Functional Requirements
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

## VR Riding Non-Functional Requirements
1. Product constraints: Device must be able to support VR and users must know how to operate a VR application. 
2. Organizational Constraints: Organization is only able to invest in certain VR headsets and not give the full experience. 
3. External constraints: Environment and knowledge in VR application.   
4. Product must be user friendly and easy to understand so that users are able to use it intuitively without much guidance.
5. System shall ensure only authorized users can access edit page. 
6. System shall ensure that users are able to understand and finish the levels and provide help/hints when needed. 
7. System shall give encouragement when users answer a question correctly.

## Setup 

### Project URL
* [Project Link: Google Drive](https://drive.google.com/open?id=1HVzAYGdR2tUlPMDpsFwt39b-0ySC7_s4)

### Dependencies

* [*GoogleVR*](https://github.com/googlevr/gvr-unity-sdk) - For character control, event control & trigger
* [*Android API level 19 and Above*](https://developer.android.com/studio/) - Android SDK

### Installation
#### Windows
1. Download Unity Hub and run 
2. Install Unity3D from Unity Hub
3. Run Unity Hub > Open > Located and select “VRsafeRiding” folder
4. Click on "Play" button in Unity3D

#### Android
1. Install VRsafeRiding_1.0.apk file 

## User Manual
### Admin Manual
*   Select "SCTF Admin" option
	* To view player analytics 
       1. select "View Analytics"
	* To set game setting 
      1. select "Game Setting"
      2. select "Game Level" (1 - 5)
      3. select desired number of vehicles,pedestrian, traffic lights and environment
  
### Player Manual
1. Select "Player" option
2. Select "Level" option (1-5)
3. Select "Vehicle" option
4. Select "Play" option

### Developer Manual
1. All the elements displayed (included vehicle, buildings, pedestrian and etc) in the game are located in the “VRsafeRiding ” > “Assets” folder
2. All the backend C# scripts are located in the “VRsafeRiding ” > “Assets” > “Scripts” folder

### Game Rules
 1. Answer all 8 quiz questions in the game which are located all over the map
 2. Avoid hitting pedestrians as well as getiing hit by vehicle and pedestrian 
    in the game
 3. Each question act as a checkpoint(save game progress) in the game 
 4. To restart the game, click on the restart menu located the at the start of the map .

## Demo
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/tC1cVljr4Yc/0.jpg)](https://www.youtube.com/watch?v=tC1cVljr4Yc)  
*Youtube Link: https://youtu.be/tC1cVljr4Yc*

## Contributors

*  _Cao Chenxing - Quiz logic_
*  _Han Yu Fong Joseph - Scene Change logic_
*  _Jeremy Tan Teng Tat - Game Menu Logic_
*  _Lim Jia Hui Alissa - Save User State logic_
*  _Lim Yoong Jin - Night Mode Logic_
*  _Ng Zhi Yuan - Traffic Light Logic_


## Errors and bugs
   1. If player is riding with the phone tilted up, he may ride out of the map
   2. Player is not facing the quiz question when he changes scene
   3. Player's screen camera and his bicyle is able tilt up/down 90 degree at the same time
   4. Vehicles and pedestrian are travelling forward and backward without turning direction
   5. Pedestrian is able to push player away whenever they hit each other.
   6. There is a "delay" time when changing between scenes.
   7. When user changed to quiz scene, the game scene is not at the pause state.
   
   
## Limitations
   1. There are no traffic rules implemented in the game, but you encouraged to adhere to them to score more points!
   2. VR-riding currently only supports android mobile
   3. Player's Phone has to be in left screen orientation 

## Feedback
   1. Implement a score system to allow player knows his statistics
   2. Implement a Health Point system 
      * Player lose a portion of his health whenever he hitted by vehicle and eventually lose the game if his health runs out
   3. Implement Play-Time Limit system
      * If player unable to finish the game with time limit give, he loses the game

## Copyright and attribution

Copyright (c) 2018 2101Team2. Released under the [MIT License](https://github.com/lewisccx/Team2/blob/master/LICENSE.MD).
