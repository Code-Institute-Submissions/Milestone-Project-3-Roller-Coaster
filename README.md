# Roller Pro Database

This is a site where both roller coaster fans and those who have a casual interest in rollercoasters can create a new dictionary of words The aim of the site is to create a databse of terms that are common to hear when discussing rollercoasters for both ethusaisnts and non ethusiasts. Scope of terms is limited to rollercoasters as these are the most common rides in a theme park.

## User Experience
* Users can create an account.
* Users can edit edit, delete and add new terms to the database
* Users can learn about common terms used to describe rollercoasters.


* Features to implement
1. Adding comments and star ratings to the terms so users can help to improve them.
2. Adding the functionality to add images to the terms. This will help users visualise the element described.
3. Create a forum where users can meet to discuss aspects of coasters and share news.
4. Link the database to YouTube and offical theme park links. The aim is to increase awareness of the parks and rides.
5. On a user's profile show them the terms they have created. Users can see the words they have created on the home page after they log in.


### Wireframes
[Desktop Home]()
[Smart Phone Home]()


## Technologies used
#### Languages used
1. [HTML 5](https://html.spec.whatwg.org/multipage/)
2. [CSS 3](https://www.w3.org/Style/CSS/Overview.en.html)
3. [Javascript](https://www.javascript.com/)
4. [Python 3.8.12](https://www.python.org/) 

#### Frameworks, Programs and Libraries used

1. [Materialize](https://materializecss.com/) Used to aid responsiveness of the site

2. [Heroku](https://www.heroku.com/) Used to deploy the finished site

3. [Gitpod](https://www.gitpod.io/) Used Gitpod for version control.

4. [Github](https://github.com/) Used to deploy the finished site.

5. [Balsamiq](https://balsamiq.com/) Used Balsamiq to create the wireframes.

6. [MongoDB](https://www.mongodb.com/) Used as a database

7. [Pep8](PEP8 online) Used to see if Python code was PEP 8 Compliant

## Testing
* The code was inputted through the W3C CSS Validation Service, Markup Validation Service and JSHint and no errors were found.
* Python was ran through Pep8 validator and no issus were found.  
* Lighthouse reports were created.
* Testing was done at each stage to ensure that the database could be mainipulated.
* User dave15 was me testing that I can create, update and delete entries.
* The website was tested on Google Chrome, Edge and  Firefox using the deployed link.
* The website was also tested on Samsung Tab S7 and Samsung S20 Ultra. 
* Family tested the deployed link on their phones and provided feedback. 

## Bugs in Testing
* Database terms were not appearing in the site when they were edited.
  This was resolved by changing the field to match the terms.  
* When searching by letter, you cannot search for A as Mongo does not allow search terms for A on its own.


#### Screenshots

Taken using the website Am I responsive
[Screenshot]()

#### Lighthouse reports
* [terms.html]()
* [login.html]()

## Deployment
The project was deployed to Heroku using the following steps...

1The following procedure was used for deployment on Heroku:

1. In Gitpod run
    pip3 freeze --local > requirements txt
    This create a requirements.txt file containing project dependencies.

2. Save the file.

3. Create a new file called Procfile 

4. Open the Procfile. Inside the file, enter:
   web: python3 app.py

6. Save the file.

7. On Heroku, sign in using your username and password.

8. On Heroku Dashboard, press the "New" button, then select "Create new app".

9. Enter the app name (note: name must be unique!) and select your region.

10. Press "Create app".

11. Go to Settings and click on Github under deployment method

12. Add your repository name then click 'Search'. Once it finds your repo, click to connect to this app.

13. On Heroku App Dashboard, select the Settings tab.

14. Click on the 'Settings' for your app, and then click on 'Reveal Config Vars'

15. Add the following variables: 
* IP: 0.0.0.0. 
* PORT 5000.
* SECRET_KEY, copy that from the env.py file, then paste it into Heroku.
* If you have MONGO_URI string fill it in, if not leave it blank.
* Add MONGO_DBNAME, this is the name of your database

16. Go back to Githjub and Add the requirements file.

17. Then commit the file

18. Add the Procfile

19. Then commit the Procfile

20. Then push in order to update GitHub.

21. Go to Heroku and now enable 'Enable Automatic Deployment'

22. Click Deploy Branch.

23. When complete you will see "Your app was successfully deployed."

24. Click "View" to launch your new app.

* The Link to the project is -(https://niall-project-roller-coaster.herokuapp.com/)

### Credits and Acknowledgments 
1. The project was heavily based on the TaskManagerAuth mini project in the Code Institute Backend Development Module. The overall structure was based on this project. Link to the repositry is -(https://github.com/Code-Institute-Solutions/TaskManagerAuth)
2. I would also like to thank my Mentor, Chris Quinn for his advice and help. I would also like to thank the tutors at Code Institute for their help.