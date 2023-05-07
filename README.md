 # Unit_4_repo
![ISAK THINK TANK1](https://user-images.githubusercontent.com/111752809/230762338-8bac8895-1e9b-4532-9e7f-cb875409876d.png)


 # Criteria A: Planning:
 ## Problem definition
 My client is a grade 11 student that studying the International Baccalaureate diploma program at their school. Despite them having access to numerous online resources, they and there pear students often struggle to find a supportive community of memebers who can help them study effectively and navigate their individual academic challenges<sup>1</sup>. This casues them to often feel isolated and overwhelmed at times of adversity, particularly when studying alone, which can negatively impact their motivation, learning goals, and in some cases their mental health. Thus the client wishes there was a way that can allow students to connect and work together in a collaborative learning enviroment<sup>2</sup> where they may discuss academic problems and help each other work their own problems out<sup>4</sup> and sharing their own resoruces<sup>3</sup>. However the client along with other students often feel embaresed with some of the question they want to ask<sup>6</sup>. They have also expressed their difficulies in finding resources for studying in the international Baccalaureate system<sup>5</sup>. The client believes that if these problems are addressed accordingly that it will foster a sense of community, allowing for their and others students academic growth and engagement, and general improvement in academic performance.
 ## Proposed Solution
 To Create a social network for the client and there school using python, html, and css along with sql databases. It will have seperate pages based off of classes a certain individual takes. These pages will allow students to communicate with their peers and share resources. They can also create their own groups to which their peers can join if they need to complete a project or group task. 
 ## Success Criteria
 
1. Allow users to create accounts and login <sup>1</sup>

2.Allow users to chat bettween eachother and in relative classes using a posting method 

3.Allow for users to upload and share resources

4.Allow users to comment on specific posts 

5.Integrate a resources page based off interests

6. Allow user to have the option to post anonymous

 ## Rationale for Proposed Soultion
Based off the clients requests and success criteria that have decided upon the next step is the development of such social network. For doing so I have decided on using Flask as the web framework, html as the standard markup language, and css as the sheet style language. These particular tools have been chosen to build the the social netowork due to their appealing traits.

Flask which is written in python syntax is a lightweight web framework that allows for developers to easily and quickly build web application with a wide range of features fexibility. This is particulary apealing for such a program due to the clients time constraint and relativly simple requirments and needs. This is better than many other web frameworks that are more complicated and require more time for development

HTML was chosen as the standard markup language for this particualr project as it is considered the industry standard for any programs that are build for web browsers. Due to its popularity it means that it is widly supported acoross many web browsers and has many online resoureces to help increase the speed of development and functionality of the social network for the client.

CSS similarly to the reason was HTML is being used CSS is the most popular method for styling formating of websites. Its vast possiblitiyes of custimization allow for any of the clients needs to be met accordingly. Also the ease of integrating CSS with HTML will allow for developers to easily and effectivly meet specific requirments of thge client.

By using Flask, HTML, and CSS I as a developer will have full control over all of the aspects of the program allowing me to fully meet any of the clients requirments in terms of design and functionality. While not comprimising on time constrains or developer setbacks that may occur if other methods were to be used. 

 # Criteria B: Solution Overview:
 ## Flow Chart
 
 ![Flow chart 1 Posting drawio (1) drawio](https://user-images.githubusercontent.com/111752809/236625415-e93e11ce-edb3-4425-b84f-e6f297bf4c8f.png)
 flow chart 1
![flow chart 2 drawio](https://user-images.githubusercontent.com/111752809/236625439-ee1d4024-4601-4044-9ea4-d92571f67cdd.png)
flow chart 2
 
 ![flow chart 3 drawio](https://user-images.githubusercontent.com/111752809/236625402-eb01b634-89a3-4d9c-a499-1b6bdb6b2a78.png)
 flow chart 3
 
![Final ER1 drawio](https://user-images.githubusercontent.com/111752809/236625450-084cddd6-87b4-4dd4-ad63-418f7a3d5522.png)
ER diagram

![uml12 drawio](https://user-images.githubusercontent.com/111752809/236625886-87d4b502-19aa-429d-ba5d-9e75883280b4.png)

UML diagram

![Final wireframe drawio (1)](https://user-images.githubusercontent.com/111752809/235333678-9c327194-4064-4ed2-883c-f4e8af9e7c74.png)
wirefram diagram
![Output App screen (2)](https://user-images.githubusercontent.com/111752809/235333733-c8d8a0ea-76fe-4d2a-b917-14adaeb59f55.png)
system diagram

 ## Test plan
 | Instruction   | Process                                            | Planned action                                                                                                                                         | Planned Outcome        | Type | Success Criteria |
|----|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------------|-----------------|
|  Login  | logging in                              | to login to users account | user able to login     | Unit test      |  1 |
|  Registration  | registering | allow user to register | user able to register account   | Unit test      |  1 |
|  Classes/posting  | entering classes                            |entering seperate classes and posting | serpated normally     | Integration testing     | 2 |
|  Uploading Resources  | entering resorces| images and resources are uploarded properly | images entered     | Integration testing      | 3 |
|  Commenting  | entering comments     | allow users to comment | users can comment    |Integration testing      | 4 |
|  Anynous output  | users can post anymous                              | users can comment | the comments work     | Integration testing     | 6 |
|  Usability  | functions             |  for function work accuratly and fast as expected | acomplished     | Non-functional testing     | 1,2,3,4,5,6 |
 ## Record of tasks

|    | Planned Action                                            | Planned Outcome                                                                                                                                         | Design Cycle      | Time Estimate      | Completion Date | Criteria |
|----|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------------|-----------------|----------|
|  1  | Completing Problem Definition                              | Creating a description for the problem from the client and their special needs | Planning     | 30 minutes      | April 9 | A |
|  2  | Creating sucesss critiera  | Creating a set of criteria that need to be met for the all of the clients requests to be satisfied| Planning     | 30 minutes      | April 13 | A |
|  3  | Proposed soultion  | The first propistion for a soultion for the clients problem. It covers all of the nessisary concerns that were rasied in the client developer meetings |Planning    | 20 minutes      |  April 14 | A |
|  4  | rationale  | Providing the reasoning for the all of the tools what are to be used in the development aspect of this Social Network. And their why I chose these tools compared methods out for web development|Planning    | 45 minutes      |  April 15 | A |
|  5  | ER diagram  | A visual diagram for the databases in the Social Network and how they work together  |Designing    | 30 minutes      |  April 16 | A |
|  6  | System diagram  | This is a visual diagram that represents the process that the users computer and server go through for the Social Network to function properly|Designing  | 45 minutes      |  April 16 | A |
|  7  | Wireframe diagram  | This is a basic representation in a diagram of all the web pages and buttons with their repsetive function and how they all work together  |Designing   | 30 minutes      |  April 16 | A |
|  8  | Login developemnt  | Creating a simple login screen that allows the user to enter the Social Network on their individual accounts by inputing their credentials |Development   | 1 hour      |  April 16 | A |
|  9  | Registration development  | Creating a Page where the new users can create a new account for the Social Network by entering their credentials. That will be sequrly stored in the servers database|Development    | 1 hour 30 minutes      |  April 17 | A |
|  10  | Database implemetation  | Connecting the registration and Login via a database that stores all of the users data and credentials|Development    | 1 hour      |  April 17 | A |
|  11  | Menu Page development  | Creating a simple and user friendly UI for users to navigate across the social network |Development    | TBD      |  April  | A |
|  12  | Classes Page development  | This a page where users can join specific descussion groups based on classes they may be taking or interested in |Development    | TBD      |  April   | A |
|  13  | Resources Page development  | This is a general page where there will be resources for students that are pre-entered how ever users pay also add their own resources they find |Development    | TBD      |  April  | A |
|  14  | Classes page developments  | The differant class buttons are made to show the discussions for each class based on whats in the database  |Development    | 1 hour 30 minutes      |  April 19 | A |
|  15  | Creating function for posting information  | Create a button whihc leads to a page that allows users to post information with a title, and content |Development    | 1 hour 30 min      |  April 19  | A |
|  16  | Improving Visuals of classes page   | To add some styling to the classes page to make it more visualy appealing   |Development   | 1 hour      |  April 19  | A |
|  17  | Adding resources page   | Add a page with many helpful resources for students that are particularly sutited for IB  |Development   | 1 hour      |  April 21  | A |
|  18  | Login authorization  | Implemenmting cookies to make the website mroe sequre for users. |Development   | 1 hour      |  April 21  | A |
|  19  | Implementing Commenting database  | Creating a database that is for holding comments connected to each post.   |Development   | 1 hour      |  April 22  | A |
|  20  | Commenting integration  | Creating a commenting page and make the nessicary connection bettween the database and post. alos inproving the UI of the commenting page  |Development    | 1 hour      |  April 27  | A |
|  23  | Adding Image uploading | Adding the feature for users to select images from their computer and upload them along with their posts   |Development   | 3 hour      |  April 29  | A |
|  24  | Code optimization  | Clearing up the code and removing repetitiveness.   |Development   | 1 hour      |  May 2  | A |
|  25  | GitHub work  | Working on do documentaion for the project  |Development    | 1 hour      |  May 5  | A |


 # Criteria C: Development:
 ## Existing tools
 | Software/Development tools| Libraries|
 |---------------------------|----------|
 |Python                     |          |
 | Flask                     | Flask              |
 |===========================| render_template    |
 |===========================| request            |
 |===========================| redirect           |
 |===========================| url_for            |
 |===========================| make_response      |
 | my_lib                    | database_worker    |
 |===========================| encrypt_password   |
 |===========================| check_password     |
 | flask_login               | LoginManager       |
 |===========================| login_user         |
 |===========================| logout_user        |
 |===========================| login_required     |
 |===========================| UserMixin          |
 | flask_wtf                 | FlaskForm          |
 | wtforms                   | FileField          |
 | =========================== | SubmitField        |
 | werkzeug.utils            | secure_filename    |
 | wtforms.validators       | InputRequired      |

 ## List of techniques


 # Criteria D: Functionality:


 ## Citation

 

 ## Apendix
 ### Client Meeting notes

 ## Final Python Code
