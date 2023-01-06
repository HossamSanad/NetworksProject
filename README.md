# Anonymous

## Project Title: E-Learning Website

## Description:
This is an online learning platform that offers access to online courses. Such a platform aims to aid any student to improve their knowledge and broaden their horizon with any speciality of interest.

## Motivation:
Our aim as a team is to boost our web development skills in order to increase our chances in finding internship/job opportunities. Moreover, providing ease of access to various courses for passionate students.

## Build Status:
The website is fully working but there is still some functionalties not finished or not fully working yet which are:
1) The quiz rendered for all the courses are the same .
2) Progress for individual,corporate trainees are not updated as they move on through course videos, hence certifcate they recieve on completing the course is not working .
3) We still need to make an equation for calculating instructor monthly income through counting courses he gave and number of enrolled trainees in his/her courses.
4) We still need to add option of a trainee to rate an instructor in the frontend.
5) We still need to make instructors, corporate trainees and individual trainees to follow up on unresolved problems.
6) We still need to adjust the salary of the instructor per month depending on the students enrolled.
7) We still need to adjust the progress of the Student's course depending on completing the course lessons.


## Code Style:

**JavaScript**
- Two spaces indentation.
- Single quotes are preferred over double. Reason: HTML uses double quotes.
- Write code in functional style with minimum side effects.
- Looping and control structures were used to aid in the understanding of the program's execution flow by those reading the code. 
- Simple statements including assignments were used to improve the flow of the code.
- Left-hand comparisons were used to place constants or expressions to the left in any comparison.
- Relationships were indicated with the association of keywords and function names with their arguments.
- Don't use function statements. Instead, create anonymous functions and assing them to vars for consistency with other vars.
```http
// No
function x(a, b) {return a * b;}

// Yes
var x = function(a, b) {return a * b;};
```
- Avoid global vars where you can. If you use them, specify it explicitly.
```http
window.globalVar = ...;
```
- Use one ```var``` per variable.
```
// Yes
var a = 5;
var b = 6;

// No
var a, b, c, d, $this;
```
- Event callback should name event data variable as 'e', not 'event' etc.

```
onChange = {(e) => setFirstname(e.target.value)}
```

- Use quotes in object keys.
```
// No
{a: 'testtest'}
// Yes
{'a': 'testtest'}

```
- Use '===' for comparing instead of '=='. JavaScript is weakly typed language, so 5 == '5'. This ambiguity could lead to hard-to-find bugs.

```
if (a === 5) {
  ...
}
if ($(this).val() === 'something') {
  ...
}
if (typeof a === 'undefined') {
  ...
}

// Exception: this compares both to 'null' and 'undefined'.
if (item == null) {

}
```
**CSS**

- Two spaces indentation.
- Use color names (e.g. white) instead of  lowercase hex colors (e.g. #fff).
- Use * {box-sizing: border-box;}.
- Use hyphens between class names, not camelCase or under_scores.
- Use only classes for styling most of the time (no #ids, elems etc).
- minimal use inline styling.
- Profile your selectors with webkit inspector.

```
.signUpCard {
  width: 450px;
  margin-left: 950px;
  color: black;


```
- Use this sequence of properties
```
.item {
  position: static;
  z-index: 0;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;

  display: block;
  visibility: hidden;
  float: none;
  clear: none;
  overflow: hidden;
  clip: rect(0 0 0 0);

  box-sizing: content-box;
  width: auto;
  min-width: 0;
  max-width: 0;
  height: auto;
  min-height: 0;
  max-height: 0;
  margin: 0;
  padding: 0;

  table-layout: fixed;
  empty-cells: show;
  border-spacing: 0;
  border-collapse: collapse;
  list-style: none;

  font: 1em sans-serif;
  font-family: Arial, sans-serif;
  font-size: 1em;
  font-weight: normal;
  font-style: normal;
  font-variant: normal;

  content: "";
  cursor: default;
  text-align: left;
  vertical-align: top;
  line-height: 1;
  white-space: normal;
  text-decoration: none;
  text-indent: 1;
  text-transform: uppercase;
  letter-spacing: 1;
  word-spacing: normal;

  opacity: 1;
  color: #d00;
  text-shadow: 5px 5px 5px #d59;
  border: 1px solid #d00;
  border-radius: 15px;
  box-shadow: inset 1px 0 0 #fff;
  background: #fff url("../i/bg.png") no-repeat 0 0; }
```


## Screenshots:
This is the home page 
![Screenshot (319)](https://user-images.githubusercontent.com/68378475/210181329-bfe50ebe-595e-40c3-87c0-b8a0fc9401d6.png)
This is a Course preview page
![Screenshot (320)](https://user-images.githubusercontent.com/68378475/210181510-4b4cfce5-c43c-4718-ae79-2511e096f87a.png)


## Tech/Framework used:

### MERN Stack:
- MongoDB
- Express framework 
- ReactJS
- Node.js

**Client:**
- React 
- Axios
- MUI
- Mongoose
- React Stripe
- JSPDF
- Bootstrap

**Server:**
- Node
- Express
- MongoDB
- Bcrypt
- Cors
- JWT
- Nodemailer
- Stripe
- Validator

## Features:

### Instructor Features:
- Log in using username and password
- Log out
- Change his/her password
- Receive an email to change a forgotten password
- Select their country
- View all the titles of the courses available including the total hours of the course.
- View the price of each course.
- Filter the courses based on a subject or rating or price
- Search for any course based on course title or subject or instructor
- View a preview video of the course
- View all the titles of the courses given by him/her.
- Filter the courses given by him/her based on a subject or price
- Search for a course given by him/her based on course title or subject or instructor
- View the ratings and reviews on all his/her courses.
- Create a new course and fill in all its details inclding title, subtitles, price, total hours, discount, subject and short summary about the entire course.
- Upload a video link from YouTube under each subtitle and enter a short description of the video.
- Upload a video link from YouTube as a preview to the course.
- Create a multiple choice exam with 4 choices per question.
- Set the answers which are not visible for the trainee for multiple choice exercises.
- View his/her rating and reviews.
- Edit his/her mini biography or email
- Define a promotion for the course and for how long
- Report a problem with a course. The problem can be "technical", "financial" or "other"
- See all previously repoted problems and their statuses

### Individual Trainee Features:
- Log in using username and password
- Log out
- Change his/her password
- Receive an email to change a forgotten password
- Select their country
- View all the titles of the courses available including the total hours of the course.
- View the price of each course.
- Filter the courses based on a subject or rating or price.
- Search for any course based on course title or subject or instructor
- View a preview video of the course
- Enter their credit card details to pay for a course they want to register for and thenpaying for this course.
- Open all the items inside a course he/she is registered for including videos and excercises.
- Rate an instructor 
- Rate a course
- Solve a multiple choice exercise by choosing the correct answer in any registered course
- Submit the answers to the exercise after completing it
- View his/her grade from the exercise
- Watch a video from a course he/she is registered for
- Write notes while watching the video
- Download the notes as a PDF
- See a list of all the courses he/she is enrolled in on their profile
- Report a problem with a course. The problem can be "technical", "financial" or "other"
- See all previously repoted problems and their statuses

### Corporate Trainee Features:
- Log in using username and password
- Log out
- Change his/her password
- Receive an email to change a forgotten password
- Select their country
- View all the titles of the courses available including the total hours of the course.
- Filter the courses based on a subject or rating.
- Search for any course based on course title or subject or instructor
- View a preview video of the course
- Open all the items inside a course he/she is registered for including videos and excercises.
- Rate an instructor 
- Rate a course
- Solve a multiple choice exercise by choosing the correct answer
- Submit the answers to the exercise after completing it
- View his/her grade from the exercise
- Watch a video from a course he/she is registered for
- Write notes while watching the video
- Download the notes as a PDF
- See a list of all the courses he/she is enrolled in on their profile
- Report a problem with a course. The problem can be "technical", "financial" or "other"
- See all previously repoted problems and their statuses

### Guest Features:
- Sign up for an account as an individual trainee using a username, email, password, first name, last name and gender.
- View all the titles of the courses available including the total hours of the course.
- Filter the courses based on a subject or rating or price.
- View the price of each course.
- Search for any course based on course title or subject or instructor
- View a preview video of the course

### Admin Features:
- Mark reported problems as "resolved" or "pending"
- Set a promotion for specific courses or several courses
- View course requests from corporate trainees
- Add another administrator with a set username and password
- Add instructors and create their usernames and passwords
- Add corporate trainees and create their usernames and passwords
- Grant corporate trainees access to specific courses

## Code Examples:
This is a function for an instructor reporting a problem:    

const reportAProblem = async(req,res) => {
    const id = req.params.id;

    const TypeOfProblem = req.body.TypeOfProblem
    const Problem = req.body.Problem
   

    try{
        const prob = await ReportedProblems.create({TypeOfProblem, Problem});
        console.log(prob);
        const inst1 = await Instructor.findById(id).populate('ReportedProblems');
        inst1.ReportedProblems.push(prob);
        await Instructor.findByIdAndUpdate(id,{ReportedProblems : inst1.ReportedProblems},{new:true}).populate('ReportedProblems'); 
        console.log(prob._id);
        console.log(inst1);
        res.status(200).json({"ReportedProblems" : inst1.ReportedProblems});
    }
    
    catch(error){
        res.status(400).json({error: error.message})
    }

 }
 

 Running such function will get the following output:
 ![Screenshot (318)](https://user-images.githubusercontent.com/68378475/210174048-42d1b38d-5d8a-4dad-a905-4cd5cc5f6661.png)
 

## Installation:

### For installation, do the following:
1- Make sure you downloaded and installed VScode \
2- Make sure you downloaded and installed node.js \
3- Clone the repository from the master branch and save it in some folder (FolderX)\
4- Open the your terminal and type in the next commands


```bash
  cd <FolderX's path folder by folder until you get there>
  npm install //this installs missing dependencies
```
Go to 'Backend' Folder> create a new file call it '.env' and add the following code lines: 
```bash
PORT = <port number> 
MONGO_URL = "<your MongoDB collection's URL>"
SECRET = <your secret pass>
STRIPE_SECRET_KEY= "<Your Stripe Secret Key"
```


Now add another terminal to your VScode.\
In one terminal add the next commands: 

```bash
  cd backend
  nodemon app.js
```

In the other terminal add the next commands:

```bash
  cd frontend
  npm start
```
A webpage will be opened automatically in your default browser.\
Now Welcome to Anonymous Website!! 🤩

## API reference:
#### GET instructor's course's titles 

```http
  GET /viewcourses/:id
```

|Parameter   | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

#### GET: Instructor filtering his/her courses by subject

```http
  GET /filtercourse/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

#### GET: Instructor filtering his/her courses by price

```http
  GET /filtercoursebyprice/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### GET: Instructor searching for courses of another instructor by instructor's name

```http
  GET /searchcourseName/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### Get: Instructor searching for his/her courses by subject ot title

```http
  GET /searchcourseSubjectandTitle/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |



#### Get: Instructor viewing the ratings of all of his/her courses

```http
  GET /viewRatings/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### Get: Instructor viewing the reviews of his/her courses

```http
  GET /viewReviews/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### Get ratings of the instructor

```http
  GET /viewMyRatings/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### Get reviews of the instructor

```http
  GET /viewMyReviews/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

#### Get view net profit per month for instructor

```http
  GET /viewMySalary/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### POST: instructor creating a course
```http
  POST /createcourse/:id
```
  
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Hours` | `number` | **Required**. course hours|
| `Title` | `string` | **Required**. course title|
| `Major` | `string` | **Required**. course subject|
| `Discount` | `string` | **Required**. course discount|
| `Subtitles` | `array` | **Required**. course subtitles|
| `Price` | `number` | **Required**. course price|
| `ShortSummary` | `Array` | **Required**. course short summary|

#### POST: instructor editing his/her email
```http
  POST /editEmail/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Email` | `string` | **Required**. new email of instructor|


#### POST: instructor editing his/her biography
```http
  POST /editBiography/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Biography` | `string` | **Required**. new biography of instructor|


#### POST: instructor defining a new promotion for one of his/her course
```http
  POST /editDiscount/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Discount` | `string` | **Required**. new discount of course|


#### POST: instructor reporting a problem

```http
  POST /reportAProblem/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `TypeOfProblem` | `string` | **Required**. type of the reported problem whether fincancial or technical or other|
| `Problem` | `string` | **Required**. Problem|


#### POST: individual trainee reporting a problem

```http
  POST /reportITProblem/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. individual trainee's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `TypeOfProblem` | `string` | **Required**. type of the reported problem whether fincancial or technical or other|
| `Problem` | `string` | **Required**. Problem|

#### POST: corporate trainee reporting a problem

```http
  POST /reportCTProblem/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. corporate trainee's id |

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `TypeOfProblem` | `string` | **Required**. type of the reported problem whether fincancial or technical or other|
| `Problem` | `string` | **Required**. Problem|

#### POST: corporate trainee requesting access to a specific course

```http
  POST /Requestaccess/:id/:id1
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. corporate trainee's id |
| `id1` | `string` | **Required**. course's id|


#### GET: admin viewing access requests 
```http
   GET /viewRequestedCourses/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. Admin's id |


#### POST: Admin grant corporate trainee access to specific courses

```http
  POST /GiveAccess/:id
```


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. Admin's id |


#### GET total enrolled students in all courses of the instructor

```http
  GET /viewTotalEnrolled/:id
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### GET reported problems of the instructor

```http
  GET /viewReportedProblems/:id
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. instuctor's id |


#### GET reported problems of an individual trainee

```http
  GET /viewITReportedProblems/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. individual trainee's id |


#### GET reported problems of a corporate trainee

```http
  GET /viewCTReportedProblems/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. corporate trainee's id|


#### GET: admin viewing all reported problems

```http
  GET /viewAllReportedProblems
```

#### POST: admin resolving a problem

```http
  POST /resolveProblem
```

#### POST: admin pending a problem

```http
  POST /pendingProblem
```

#### POST: admin setting a promotion for several courses

```http
  POST /setPromotion
```

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Price` | `number` | **Required**. price of several courses|
| `Discount` | `number` | **Required**. promotion for courses|

#### POST: admin setting a promotion for a specific course

```http
  POST /setSpecificPromotion
```

| Body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Title` | `string` | **Required**. Title of the course|
| `Price` | `number` | **Required**. price of the course|
| `Discount` | `number` | **Required**. promotion for the course|

#### GET the progress of an corporate trainee

```http
  GET /GetCorporateProgress/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. corporate trainee's id|


#### GET the progress of an individual trainee

```http
  GET /GetIndividualProgress/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. individual trainee's id|


## Tests: 
-We tested the website using different accounts with different roles to test all the features so everyone in the team verified the functionlities several times in order to check if the website is working well without any problems.

### Using Postman:
- This is to test for editing the email of an instructor: 
![Screenshot (325)](https://user-images.githubusercontent.com/68378475/210799213-1d9680be-b8d5-4f6c-86ad-eb055bb6753f.png)

- This is to test for setting a promotion for a specific course and the price of such course will be changed depending on the promotion:
![Screenshot (326)](https://user-images.githubusercontent.com/68378475/210799605-b5d36b31-900e-466d-bc81-05c6a1db1d19.png)

## How to use: 
1) You will view the website as a guest at first and you can sign up for the full access.  
2) Log in and you will have the home page where you can see search bar in top right corner to search any course and you can also filter.
3) Depends how you signed up as an individual trainee , corporate_trainee , instructor or Admin you can access what you need in the navigation bar at the top.
4) You will have everything clear for what you want to do as everything is labelled well.

## Contribute:
[Contributor Covenant](contributing.md)

## Credits:
I would like to thank my Team for the effort done and our Project Manager Noha Abdellatif for the support :)
 ### The Team : 
 - Mazen Fayad : https://github.com/MazenFayad
 - Hossam Sanad : https://github.com/HossamSanad
 - Omar Warda : https://github.com/OmarWarda
 - Mazen Alaa : https://github.com/Mazen2001-del
 - Eslam Hany
 ### Source I learned from : 
[Tutorials](https://youtu.be/98BzS5Oz5E4) 





## License: 
 - [MIT License](LICENSE)
 - Stripe License : [Apache License](License)
  
  
  
