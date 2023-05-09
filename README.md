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

CSS similarly to the reason was HTML is being used CSS is the most popular method for styling formating of websites. Its vast possiblitiyes of custimization allow for any of the clients needs to be met accordingly. Also the ease of integrating CSS with HTML will allow for developers to easily and effectivly meet specific requirments of the client.

By using Flask, HTML, and CSS I as a developer will have full control over all of the aspects of the program allowing me to fully meet any of the clients requirments in terms of design and functionality. While not comprimising on time constrains or developer setbacks that may occur if other methods were to be used. 

 # Criteria B: Solution Overview:
 ## Data dictionaires
 ![Login data](https://user-images.githubusercontent.com/111752809/236673359-ea5125d6-662d-4ef5-b3b1-7ff7a873d5af.png)

 ## Flow Chart 1
 ![Flow chart 1 Posting drawio (1) drawio](https://user-images.githubusercontent.com/111752809/236625415-e93e11ce-edb3-4425-b84f-e6f297bf4c8f.png)
 
  **Fig-1**: Once the alorithm recives a post request begins a process of getting all of the nessisary parameters for a post. It will receive the title, content, and images take from the user input. It receives the username by first getting the user_id with the cookie then quering the user_id to database to find the username. Once all the data has been collected it will check whether the user has selected to keep the username anaymous, after which it will enter all of the data into their respective places in the database.
 ## Flow chart 2
![flow chart 2 drawio](https://user-images.githubusercontent.com/111752809/236625439-ee1d4024-4601-4044-9ea4-d92571f67cdd.png)

 **Fig-2**: On the instance a request is made the algorthm will begin by  creating a connection to the "social_net.db" atabase. The class_id is retrieved from the request arguments. After which, a query is run to collect all of data from the "classes" table based class_id. Then once all the data has been receiveed it closes the connection to the database. Then it will initializes an empty list for posts and iterates over the information from the database. For each row, a post dictionary is created and filled with given data. The post is then added to the list of posts. Finally, the function renders the class disscussion having the class_id and the list of posts as parameters.
## Flow chart 3
 ![flow chart 3 drawio](https://user-images.githubusercontent.com/111752809/236625402-eb01b634-89a3-4d9c-a499-1b6bdb6b2a78.png)
 
  **Fig-3**:flow chart 3
 ## ER
![Final ER1 drawio](https://user-images.githubusercontent.com/111752809/236625450-084cddd6-87b4-4dd4-ad63-418f7a3d5522.png)

 **Fig-4**: The ER diagram seen above is a visual representation of the relationships between entities in the social network database. It illustrates how different entities relate to each other and the attributes associated with each entity. Such as the connection bettween the user, classes, and comments tables.
## UML Diagram
![uml12 drawio](https://user-images.githubusercontent.com/111752809/236625886-87d4b502-19aa-429d-ba5d-9e75883280b4.png)

 **Fig-5**:The UML (Unified Modeling Language) diagram above shows the OOP(Object Oriented Programming) used in the database interaction bettween the social network and the sqllite database. It first initializes the name of the database entered with a connection to the given sql database. From there each of the 3 functcions; searching in the database, changing and saving information in the database, and closing the database. 
## Wireframe Diagram
![Final wireframe drawio (1)](https://user-images.githubusercontent.com/111752809/235333678-9c327194-4064-4ed2-883c-f4e8af9e7c74.png)

 **Fig-6**:The Wirefram diagram above outlines the basic structure and layout of a Social Network Webpage. It shows the basic outline and architeture of the webpages features, such as buttons and inputs. There are also colored arrows to show the relationship between the buttons the pages that they lead too. All the arrows with the same color lead to the same function or page.
## System diagram
![Output App screen (2)](https://user-images.githubusercontent.com/111752809/235333733-c8d8a0ea-76fe-4d2a-b917-14adaeb59f55.png)

 **Fig-7**: The system diagram shows the realationship bettween the server running the website and the clients screen. It shows all of the componets used for the creating the social network that are being run all the functions and visuals on the clients screen. It shows how the Social Networks communicates with the server through GET and POST requests.

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
 
 * Web development using Flask framework
* User registration and login functionality
* Handling form submissions
* Database operations (SQLite)
* File uploads and handling
* Cookie management
* Templating with Jinja2 (rendering HTML templates)
* Routing and URL handling
* Redirecting users
* Input validation with WTForms
* Password encryption and verification
* Handling HTTP requests and responses
* Cascading Style Sheets (CSS) and styling of HTML templates
 ## Refreneces
 ### Main Development Refrences
 #### AWS Code Whisper
 "CodeWhisperer is trained on billions of lines of code and can generate code suggestions ranging from snippets to full functions in real time based on your comments and existing code. Bypass time-consuming coding tasks and accelerate building with unfamiliar APIs." https://aws.amazon.com/codewhisperer/
 #### Chatgpt 3
 ChatGPT-3 is an AI language model developed by OpenAI that can provide insightful suggestions along with assisting with coding and development-related inquiries and offering suggestions on how to improve or procede with issues. It can also help provide soltions when errors or bugs are found it code.
 #### Other refrences
 # Code
 ## Login[Critiera:1]
 ```.py
@app.route('/', methods=['GET', 'POST'])
def login():
    if request.method == 'POST':
        email = request.form['email']  # Retrieve email from the form data
        passwd = request.form['passwd']  # Retrieve password from the form data
        
        db = database_worker("social_net.db")  # Create a connection to the database
        user = db.search(f"SELECT * from user where email = '{email}'")  # Search for a user with the given email

        if user:
            user = user[0]
            id, email_db, hashed, username = user

            if check_password(hashed_password=hashed, user_password=passwd):  # Check if the password is correct
                response = make_response(redirect(url_for('menu')))  # Create a redirect response to the 'menu' page
                response.set_cookie('user_id', f"{id}")  # Set a cookie with the user ID
                return response

    return render_template("login_screen.html")  # Render the login template
 ```
 The code above is one part of the first success criteria that being allowing users to login with their respective accounts. The algorthim goes through many conditional statements and logical checks to ensure the data entered by the users is correct and corelated to what is stored in the database. Through this process it will check whether the password entered maxes the encrypted password in the database. Once these set of Condional statements are met then the user is redirected to the menu page. Some difficulties with code involved figuring out the order of the tasks as everything needs to be done at the correct time for the program to function as intended
 ## Registrastion [Critiera:1]
 ```.py
@app.route('/register', methods=['GET', 'POST'])
def register():
    if request.method == 'POST':
        email = request.form['email']  # Retrieve email from the form data
        email_confirmation = request.form['email_confirm']  # Retrieve email confirmation from the form data
        username = request.form['username']  # Retrieve username from the form data
        password = request.form['passwd']  # Retrieve password from the form data
        password_confirmation = request.form['passwd_confirm']  # Retrieve password confirmation from the form data
        
        if email != email_confirmation:  # Check if email and email confirmation match
            return "Email confirmation doesn't match, please try again."
        if password != password_confirmation:  # Check if password and password confirmation match
            return "Password confirmation doesn't match, please try again."

        db = database_worker("social_net.db")  # Create a connection to the database
        hashed_password = encrypt_password(password)  # Encrypt the password

        query = f"INSERT INTO user (email, password, username) VALUES ('{email}', '{hashed_password}','{username}')"  # Create an SQL query to insert user data into the database
        db.run_save(query)  # Execute the SQL query
        db.close()  # Close the database connection

        return redirect(url_for('login'))  # Redirect to the login page

    # Render the register template
    return render_template('register_screen.html')
 ```
 The code above is the secodn aspect of the first Criteria being registration. Once a post request has been made by the user it will take the text inputs by the user and being an algotihm to check and process the code. The algorithm will go throught several validation checks to make sure that all the text inputs are filled correctly. One example of this the the email confrmation check that makes sure that the user has entered the correct email. Overall the code decomposes the login functionality into separate steps or subtasks that get handled. It will gor through a process of request methods, retrieving form data, performing database queries, and also checking password validity
 ## Posting [Critiera:2,6]
 ```.py
  if request.form.get('anonymous'):
    username = 'Anonymous'  # Set the username to 'Anonymous' if the 'anonymous' checkbox is checked

file = request.files['file']  # Retrieve the uploaded file from the form data

if file.filename == '':
    print('no file')  # Print a message if no file is selected

if file.filename != '':
    filename  = secure_filename(file.filename)  # Securely get the filename
    file.save(os.path.join(app.config['UPLOAD_FOLDER'], filename))  # Save the file to the specified folder
    print('file successful')  # Print a message if the file is successfully saved

if file.filename == '':
    filename = "NONE"  # Set the filename to "NONE" if no file is selected

query = f"INSERT INTO classes (class_id,Username,Title, Content, Images) VALUES ('{class_id}', '{username}', '{title}','{content}','{filename}');"  # Create an SQL query to insert data into the classes table
db.run_save(query)  # Execute the SQL query
db.close()  # Close the database connection
 ```
The code above depicts one aspect of the posting alogrithm that covers two of the success criteira. Starting from the top of the code their is Conditional statement to check whether a user has clicked a checkbox to keep their post Anoymous. As the algorthum progress it will go through many more sets of Condiotnal Statements regarding Image/resources uploading. This is an extremlty vital part that required algorithmic thinking to compltete properly. As uploading files to a server can be an extremly vunrable for a website it goes through these condiiotnal statements to ensure the saftly of the Social Network. This is where I use werkzeug.utils library and secure_filename to make sure the file is safe. After this it checks if the user has selected a image or not to properly enter a standerdised data in the database.
 ## Uploading resources [Critiera:3]
 ```.py
 <form method="POST" enctype="multipart/form-data">
    <h2>Create a Post</h2>
    <input class="hidden" type="text" name="class_id" value="{{ class_id }}"></input>  <!-- Hidden input field to store the class ID -->

    <label for="title"><b>Title</b></label>
    <input type="text" placeholder="Enter Title" name="title" required>  <!-- Input field for entering the post title -->

    <label for="content"><b>Content</b></label>
    <textarea placeholder="Enter Content" name="content" required></textarea>  <!-- Textarea for entering the post content -->

    <input type="checkbox" name="anonymous" id="anonymous" value="true">  <!-- Checkbox for anonymous posting -->
    <label for="anonymous">Keep Anonymous</label>

    <input type="file" name="file" accept="image/*">  <!-- File input field for uploading images -->
</form>
 ```
 The code above shows the html code of the posting process. The preious sample of code explored the back-end processes. However this is the frontend aspect. This partiular area was where many difficutis where encountered as I needed a way to make the distintction bettween the class_id, post_id, and comment_id. As they are all related and conntected to each otehr meaning the differation bettween classes was vital. So I employed a method of givign each class an id. However to ahve th id carry over to differant function I enter a hidden input that takes what class the user clicked and saves it here for other function. For example displaying the posts from the database and connecting them to comments. 
 ## Commenting [Critiera:4]
 ```.py
 def post_comments(post_id):
    post_id = post_id.split(':')  # Splitting the post ID into class ID and post ID
    class_id = post_id[0]
    posts_id = post_id[1]
    db = database_worker("social_net.db")  # Creating a database worker object

    # Fetching the post details from the database based on the class ID
    posts = db.search(f"SELECT * from classes where class_id='{class_id}'")

    for i, row in enumerate(posts):
        if posts_id == f'{i + 1}':
            post_title = row[3]  # Extracting the post title from the row
            post_content = row[4]  # Extracting the post content from the row
            post_username = row[2]  # Extracting the post username from the row
            post_images = row[5] if row[5] else 'NONE'  # Extracting the post images from the row, or set it to 'NONE' if it's empty
            post_comments = []  # List to store post comments

            # Fetching the comments for the post from the database
            comment_rows = db.search(f"SELECT * from comments where post_id='{i + 1}' and class_id = {class_id}")

            for comment_row in comment_rows:
                comment = {
                    'username': comment_row[2],  # Extracting the comment username from the row
                    'content': comment_row[3]  # Extracting the comment content from the row
                }
                post_comments.append(comment)  # Adding the comment to the list of post comments
            break  # Exiting the loop once the desired post is found
 ```
 This code is responsible for complteting one part of the forth criteria which is for posting commenting. The alogrithm was developemted in the process as follows.  It retrieves post details and comments based on a given post ID. It then splits the post ID into class ID and post ID, connects to the database, and gets all of the corresponding post information from the "classes" table. It then iterates over the this retirveed data and extracts the title, content, username, and images. Additionally, it will retrieves comments for the post from the "comments" table, storing them in a list. That comments go through a loop in the form of a dictionary to extract the username and content of each comment so that it will later get posed The code implements techniques such as database querying, data extraction from rows, list manipulation, and looping to retrieve the given post and its respective comments.
 ```.py
 if request.method == 'POST':
    # Retrieve the comment content from the form
    comment_content = request.form['comment']
    user_id = request.cookies.get('user_id')
    username = db.search(f"SELECT username from user where id ='{user_id}'")

    # Insert the new comment into the database
    query = (f"INSERT INTO comments (post_id, class_id, Comment_Username, Comment_Content) VALUES ({i + 1}, {class_id}, '{username[0][0]}', '{comment_content}')")
    db.run_save(query)
    db.close()

    # Redirect to the same page to refresh the comments list
    return redirect(request.url)
else:
    # Render the page with the existing comments
    return render_template('classes_discussion_post_comments.html', title=post_title, username=post_username, content=post_content, comments=post_comments, post_images=post_images)

return render_template('classes_discussion_post_comments.html', post_id=post_id, title=post_title, content=post_content, username=post_username, comments=post_comments, post_images=post_images)
 ```
 As Showing the clicked on post, its comments, and creating a new comment were all on the same page I need a way for the algorthim to go through each of the nessicary requirements such as first displaying the post along with its relative content. Then displaying all the comments in the database. Afterwards it will check whether a post comment was been requested or not. This means that once the page is renderd or a post is made the alorithm can quicky complete the nessicary tasks.
 ## Data Management [Critiera:1,2,3,4,5,6]
 ### How the Data structure System
![data_storage drawio](https://user-images.githubusercontent.com/111752809/236682444-c4a7bf57-a705-4930-9b4b-9c84e1c30434.png)
 **Fig-8**:The diagram above depicts the hierarchical relationships between classes,posts, and comments. Every class node acts as a parent code in the hierarchical relationships meaning the posts as a child node can have as many posts as the the system can physical handle. This same process occurs for comments where the post acts as a parent node to many comments which are child nodes. What this allows for is an extremly simple method to implement a new class as once a new class id has been given all the post and comments which are later created link to each other. This also means for the development of the front end aspect it only requires one page to display posts, and one to comment. As what is rendered follows the path of each class and post.
```.py
class database_worker:
    def __init__(self, name):
        # Initialize the database worker by connecting to the specified database
        self.connection = sqlite3.connect(name)
        self.cursor = self.connection.cursor()

    def search(self, query):
        # Execute the search query and fetch all results
        result = self.cursor.execute(query).fetchall()
        return result

    def run_save(self, query):
        # Execute the query and commit changes to the database
        self.cursor.execute(query)
        self.connection.commit()

    def close(self):
        # Close the database connection
        self.connection.close()
```
The code above shows how this Social Networks process how information gets too and from various data tables. This is one example where OOP(Object Oritented Programming) was used allow various functions to be called when ever needed rather than writing the whole algorithm over and over. The class has 3 methods which are responsible for handling interactions with the SQLite database. When I am initialized with a name, I connect to the specified database using sqlite3.connect. The search(self, query) method executes a given search query on the connected database, fetches all the results using the fetchall() method, and returns the fetched results. The run_save(self, query) method executes a given query that modifies the database using the execute() method, and then commits the changes to the database using the commit() method. And finally the close(self) method closes the connection to the database when it is no longer needed.
```.py
@app.route('/delete_post/<int:post_id>', methods=['POST'])
def delete_post(post_id):
    # Initialize the database worker
    db = database_worker("social_net.db")
    
    # Construct the query to delete the post with the specified post_id
    query = (f"DELETE FROM classes WHERE id={post_id}")
    
    # Execute the query to delete the post
    db.run_save(query)
    
    # Close the database connection
    db.close()
    
    # Redirect to the 'menu' page after deleting the post
    return redirect(url_for('menu'))

 ```
 The code above is an example another aspect of data management. That being keeping the data tables in the sqlite database organized and clear of any unessiary content. The functions allows users to quickly and easily delete posts that they longer wish to have. 
```.py
<form action="{{ url_for('delete_post', post_id=post['id']) }}" method="post">
    <!-- Delete Post Form -->
    <button class="trash-button" type="submit"><i class="fas fa-trash"></i></button>
</form>
```
The code above shows the Html for deleting posts. Instead of having a simple button that says delete I deceied to use a trashcan Icon to represent the delete button improve the UI experiance by keeping it minimal. This was done by refrencing this web address "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" 
 ## Formating/styling[Critiera:1,2,3,4,5,6]
 ```.py
<!DOCTYPE html>
<html>
  <head>
    <title>My Menu Page</title>
    <!-- Referencing the CSS containing style sheet -->
    <link rel="stylesheet" href="/static/Menu_style.css">
    <style>
    <!-- Base CSS for every page -->
      body {
        background-image: url('/static/background gradient.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        background-attachment: fixed;
      }
    </style>
  </head>
  <body>
    <!-- Sidebar -->
    <div class="sidebar">
      <a class="active" href="/menu">Home</a>
      <a href="/classes">CLASSES</a>
      <a href="/resources">RESOURCES</a>
    </div>
 ```
 The html code above establishes a consistent structure and style for the pages in the social network to follow, with a sidebar navigation menu and a base CSS for a background image it provieds a simple template for the UI. Other features and content can be added within the <body> section based on this template keeping pages consistent.
 
 # Criteria D: Functionality:

 ## Video Demonstration
https://user-images.githubusercontent.com/111752809/236778483-aef4f224-cb17-4fc4-acb3-71bb1dd3d926.mp4
 ## All Code
https://drive.google.com/drive/folders/18-R1u6SCh9nO37DIwpqQOOodigA2-RG1?usp=sharing
 # Criteria E
 ## Client Feedback
 |  Criteria  | ✓ / 𐄂          | Client Comments  |
|-------------|----------------|------------------|
| Allow users to create accounts and login         |  ✓              |                  |
| Allow users to chat bettween eachother and in relative classes using a posting method            |    ✓            |                  |
|Allow for users to upload and share resources             |    ✓            |                  |
|Allow users to comment on specific posts             |       ✓         |                  |
|Integrate a resources page based off interests             |       ✓         |                  |
 |Allow user to have the option to post anonymous           |        ✓        |                  |
 
 ## Random User Feedback
 |  Criteria  | ✓ / 𐄂          | Client Comments  |
|-------------|----------------|------------------|
| Allow users to create accounts and login         |  ✓              |                  |
| Allow users to chat bettween eachother and in relative classes using a posting method            |    ✓            |                  |
|Allow for users to upload and share resources             |    ✓            |                  |
|Allow users to comment on specific posts             |       ✓         |                  |
|Integrate a resources page based off interests             |       ✓         |                  |
 |Allow user to have the option to post anonymous           |        ✓        |                  |

 

 ## Apendix
 ### Client Meeting notes

