<div align="center">

<h1 align="center">Track Attendance!!</h1>

[![](https://img.shields.io/badge/Made_with-Nodejs-red?style=for-the-badge&logo=node.js)](https://nodejs.org/en/)
[![](https://img.shields.io/badge/IDE-Visual_Studio_Code-purple?style=for-the-badge&logo=visual-studio-code)](https://code.visualstudio.com/  "Visual Studio Code")
[![](https://img.shields.io/badge/Database-MongoDB-green?style=for-the-badge&logo=mongodb)](mongodb.com "MongoDB")
[![](https://img.shields.io/badge/Made_with-Python-blue?style=for-the-badge&logo=python)](https://www.python.org/)

</div>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
     <a href="#built-with">Built With</a>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
  </ol>
</details>

### Built With

* [NodeJS](https://nodejs.org/en/)
* [ExpressJS](https://expressjs.com/en/starter/generator.html)
* [Python](https://www.python.org/)
* [OpenCV](https://opencv.org/)

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

Update to the latest version of npm
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/1manasa2/trackAttendance.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Install Python packages
   
   ```sh
   cd ./Py-Scrpits 
   pip3 install requirements.txt
   ```

### Running the project
1. Start the express server from the root directory
   ```sh
   npm start
   ```
2. Start the flask server
    ```sh
    cd ./Py-Scripts
      python3 app.py
   ```
3. Start the mongo server
    ```sh
    mongod --dbpath YOUR_PATH
   ```

<!-- USAGE  -->
## Usage


#### **Home Page**: Lets take a dive into our portal!

#### **Steps for registration of a student**: 

1. Verify your email 
   
   - 6 digit OTP is sent to the entered email

(**Note:** Only college domain emails accepted)

2.  Fill the registration form



(**Note:** Cannot create account for an existing roll number)

(**Note:** Password must satisfy specified conditions)

3. Logging in student's account for the first time
   
   - Classrooms page

   - Profile page

#### **Steps for registration of a teacher**: 

1. Verify your email 
   
   - 6 digit OTP is sent to the entered email
  

(**Note:** Only college domain emails accepted as mentioned above)

2.  Fill the registration form

(**Note:** Password must satisfy specified conditions)

3. Logging in teacher's account for the first time
   
   - Dashboard page

   - Classroom page


#### **Steps for creating a new classroom**: 

1. Create a new classroom
  
   - Click "Create new classroom" on the classrooms page
   - Fill the following form 
  

2. View details
  
   - Click "See all" button of a particular classroom on the classrooms page 

   - Class details page after creating a new class

#### **Steps for manually adding a student to a new classroom**: 

1. Add students directly 

   - Click "Add students" on the class details page

    - Add any student by clicking on "+" to add a student to the class

    - After adding a student classrooms page

    - After adding a student class details page

    - Get an email notification when you are added to a class


2. Add students using filter 

   - Click "Filters" on the Add Students page
   
   - Select any filter/filters
   
   - Add any student by clicking on "+" to add a student to the class

3. Add all students at once

   - Click "Add all" button on the Add Students page (You can add all filtered students as well)

#### **Steps for joining a classroom with an unique code:** 

1. Copy code
   
   - Copy and send the unique code displayed on the class details page to students using your preferred choice of communication

2. Enter received code to join a classroom
   
   - A student will receive a code from the teacher. Using this code he can join that particular classroom by entering the code in the box displayed below
    
    - Entering wrong code

    - Entering correct code

    - Entering code of a class, of which you are already a part
  
#### **Steps for uploading a picture for face recognition:** 

**Note:** This photo will also be set as a default profile picture of your account!!

1. Upload image form

   - Open the upload image tab in the student's portal

   - Select an image in whoch your face is clearly visible (**Note:** Only jpg format is accepted and your image must have the filename as follows 'rollnumber.jpg')
  
    - The image below is blurred for privacy.

2. After uploading your image

   - Classrooms page

   - Profile page
    

#### **Steps for recording attendance:** 

Log in to your teacher's account.

1. Conduct a lecture

    - Click the "Conduct Lecture" button in the class details to conduct a lecture


    - After conducting a lecture the lecture number increases as highlighted below. After this step the teacher can start recording the attendance

2. Record attendance
  

    - Click the "Take attendance" button in the class details to start the camera and record the attendance


    - A window will open and a camera will start to record the attendance. You can press q to exit the recording frame once you are done recording the attendance
    - A notification bell sound will be heard once a student is recognised and his/her name will be displayed in the frame as shown below

**Note:** Our app supports multiple face detection in a single frame as well.

#### **Statistics based on attendance:** 

1. Dashboard
   
    - Our app calculates numerous statisitics based on the recorded attendance for the teachers to analyse. Below is a screenshot of the dashboard displaying the same.

2. Classrooms
   
      - The classroom page displays all the classrooms the teacher has created and displays various stats as displayed below.

      - The class details page will also display various stats related to the particular classroom

3. Student Portal

   - Students can view all the classrooms they are a part of, and view their individual attendance in each of the classes.

    - Students can view the classes in which they have attendance less than 75%

    - Profile of the student will also show whether they have optimal overall attendance

4. Update Details

    #### **Update Profile picture**

    - Click on the profile photo to open the form. A modal will appear and then you can select the photo of your choice.

    - Once the photo is updated, you will be notified and the change will reflect on your profile.

    #### **Update Profile details**

    - Click on the settings button to open the form. A modal will appear and then you can change the details of your choice

    - After submitting the form, the profile will be updated.

    #### **Update Class details**

    - Click on the settings button of the required class to open the form. A modal will appear and then you can change the class details of your choice


    - After submitting the form, the class details will be updated.
    

#### **Exporting to XLSX:** 

1. Attendance export
  
    - You can export the attendance to .xlsx file by clicking on the "Download Attendance button" on the sidenav.
   

    - After the download has completed, you can access the xlsx file in your downloads folder on your local computer
  

2. Absentees export

   - Open the form for entering a date by clicking on the "Absent Students" button on the sidenav
  
    - You can select a particular date to find out the people who were absent on that day along with the class name which they didnt attend. If there was a mass bunk it will be displayed as "Mass Bunk".
    
    - After selecting the date you can view the absentees


    - You can export the absentees to xlsx file and download it on your local computer by clicking on the "Download XlS File"

#### **Connect Android Device Camera:**

Setup : <br>
Step 1 : Install "IP Webcam" APP from playstore <br>
Step 2 (optional) : Go to Video preferences and select Main Camera as Front camera 

To Run : **(Both Devices should be connected to same Network)** <br>
Step 1 : Click on Start server <br>
Step 2 : Get the IPv4 address(shown on android screen). eg- 127.123.0.105:8000 <br>
Step 3 : Enter the addess in "Connect Android" Input Field.<br>
Step 4 : Click Take Attendance

![product](./images/connect_android_filled.PNG)


