# Roller Pro Database

This is a site where both roller coaster fans and those who have a casual interest in roller coasters can create a new dictionary of words The aim of the site is to create a database of terms that are common to hear when discussing roller coasters for both enthusiasts and non enthusiasts . Scope of terms is limited to roller coasters as these are the most common rides in a theme park.

## User Experience
* Users can create an account.
* Users can edit edit, delete and add new terms to the database.
* Users can learn about both common and specific terms used to describe roller coasters.

* Features to implement
1. Adding comments and star ratings to the terms so users can help to improve them.
2. Adding the functionality to add images to the terms. This will help users visualise the element described.
3. Create a forum where users can meet to discuss aspects of coasters and share news.
4. Link the database to YouTube and official theme park links. The aim is to increase awareness of the parks and rides.
5. On a user's profile show them the terms they have created, and add the functionality to add an photo of themselves. Currently Users can see the words they have created on the home page after they log in.

### Wireframes
* [Desktop Home](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/Wireframes/Desktop.png)
* [Smart Phone Home](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/Wireframes/Smart%20Phone.png)

## Technologies used

#### Languages used
1. [HTML 5](https://html.spec.whatwg.org/multipage/)
2. [CSS 3](https://www.w3.org/Style/CSS/Overview.en.html)
3. [JavaScript](https://www.javascript.com/)
4. [Python 3.8.12](https://www.python.org/) 

#### Frameworks, Programs and Libraries used

1. [Materialize](https://materializecss.com/) Used to aid responsiveness of the site.

2. [Heroku](https://www.heroku.com/) Used to deploy the finished application.

3. [Gitpod](https://www.gitpod.io/) Used Gitpod for version control.

4. [Github](https://github.com/) Used to store code and automatically deploy the finished application to Heroku.

5. [Balsamiq](https://balsamiq.com/) Used Balsamiq to create the wireframes.

6. [MongoDB](https://www.mongodb.com/) Used as a database.

7. [Pep8](http://pep8online.com/) Used to see if Python code was PEP 8 Compliant

8. [Am I Responsive?](http://ami.responsivedesign.is/) Used to provide screenshots of the site on different devices.

## Testing
* The code was inputted through the W3C CSS Validation Service, Markup Validation Service and JSHint and no errors were found.
* Python code was ran through Pep8 validator and no issues were found.  
* Lighthouse reports were created and scored over 90 on all areas that were tested.
* Testing was done at each stage to ensure that the database could be manipulated.

* User Story testing
1. Can a user create an account?
* Users are able to successfully create an account. For testing I created 3 different accounts usernames were: crazym, dave15 and admin.

2. Can users add terms to the database?
* Users are able to add terms in the database. To test this I created fake entries to the database and they appeared on the site.

3. Can users edit terms
* Users are able to edit the terms in the database. To test this I edited the fake entries.

4. Can users delete terms?
* Users are able to delete terms. In the database you cannot see any fake entries.

* On the site you can see terms entered by a user called dave15. This user is me testing that I can create, update and delete entries.
* The website was tested on Google Chrome, Edge and Firefox using the deployed link.
* The website was also tested on Samsung Tab S7 and Samsung S20 Ultra. 
* Family tested the deployed link on their phones and provided feedback. 

## Bugs in Testing
* Database terms were not appearing in the site when they were edited.
  This was resolved by changing the field to match the terms.  
* When searching by letter, you cannot search for A as MongoDB does not allow search terms for A on its own as it is a very common term.

#### Screenshots
* [Screenshot taken using the website "Am I responsive?"](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/screenshots/rollerPro.JPG)
* [Desktop Home Page](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/screenshots/Desktop-terms.JPG)
* [Smart Phone Home Page](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/screenshots/Smartphone%20terms.jpg)

#### Lighthouse reports
* [terms.html](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/Lighthouse%20reports/Lighthouse-report-all-terms.JPG)
* [login.html](https://github.com/NC-CSX/Milestone-Project-3-Roller-Coaster/blob/main/static/assets/Lighthouse%20reports/Lighthouse-report-log-in.JPG)

## Deployment
The project was deployed to Heroku using the following steps...

The following procedure was used for deployment on Heroku: This assumes that you already have created your MongoDB database

1. In Gitpod run

    pip3 freeze --local > requirements txt
    
    This creates a requirements.txt file containing project dependencies.

2. Save the file.

3. Create a new file called Procfile. 

4. Open the Procfile. inside the file, enter:
   
   web: python3 app.py

5. Save the file.

6. On Heroku, sign in using your username and password.

6. On the Heroku Dashboard, click on New, then select Create new app.

8. Enter the app name, this name must be unique, and select your region.

9. Click Create app.

10. Go to Settings and click on Github under deployment method.

13. Add your Github repository name, click Search. When your repository is found, click to connect to this app.

14. On the Heroku Dashboard, select Settings.

15. Click on Reveal Config Vars

16. Add the following variables: 
* IP: 0.0.0.0. 
* PORT 5000.
* SECRET_KEY, Copy this from the env.py file, then paste it into Heroku.
* MONGO_URI, If you already have a string fill it in, if not leave it blank.
* MONGO_DBNAME, Add the name of your database.

17. Go back to Gitpod and add the requirements file.

18. Then commit the file.

19. Add the Procfile.

20. Then commit the Procfile.

21. Then push in order to update GitHub.

21. Go to Heroku and now enable Enable Automatic Deployment.

22. Click Deploy Branch.

23. Click "View" to launch your new app.

* The Link to the application is -(https://niall-project-roller-coaster.herokuapp.com/)

### Credits and Acknowledgments 
1. The project was heavily based on the TaskManagerAuth mini project in the Code Institute Backend Development Module. The overall structure was based on this project. Link to the repository is -(https://github.com/Code-Institute-Solutions/TaskManagerAuth)
2. I would also like to thank my Mentor, Chris Quinn for his advice and help. I would also like to thank the tutors at Code Institute for their help.