# Little Lemon App


## Main Steps
1. **Create an environment:**

    **Windows:**
    ```
    python -m venv env
    ```
    **MacOS:**
    ```
    python3 -m venv env
    ```

2. **Environment activate:**

    **Windows:**
    ```
    .\env\Scripts\activate
    ```
    **MacOS:**
    ```
    source env/bin/activate
    ```

3. **Install Django:**

    **Windows:**
    ```
    pip install django
    ```
    **MacOS:**
    ```
    pip3 install django
    ```

    **Verify Django Version:**

    **Windows:**
    ```
    python -m django version
    ```
    **MacOS:**
    ```
    python3 -m django version
    ```

4. **Install Django Rest Framework:**

    **Windows:**
    ```
    pip install djangorestframework
    ```
    **MacOS:**
    ```
    pip3 install djangorestframework
    ```

5. **Start Project:**

    ```
    django-admin startproject <name> .
    ```

6. **Create APP:**

    **Windows:**
    ```
    python -m django startapp <name>
    ```
    **MacOS:**
    ```
    python3 -m django startapp <name>
    ```

    **OR**

    **Windows:**
    ```
    python manage.py startapp <name>
    ```
    **MacOS:**
    ```
    python3 manage.py startapp <name>
    ```

7. **Run Server:**

    **Windows:**
    ```
    python manage.py runserver
    ```
    **MacOS:**
    ```
    python3 manage.py runserver
    ```

8. **Migrations:**

    ```
    python manage.py migrate
    ```

9. **Create Super User**

    ```
    python manage.py createsuperuser
    ```

    ```
    admin
    Email address: django@python.com
    Password: 12345678A@
    ```


## Overview
By working through the lessons in this course, you've learned the necessary skills and knowledge to develop back-end APIs for the Little Lemon project. You were provided with code snippets and your task was to use these, plus any of your own code, to complete an API project for the Little Lemon restaurant.

You will now take part in a peer-review exercise in which you will submit your completed APIs for two of your peers to review. You will also be required to review two of your peers' projects.

Detailed criteria are covered in the grading criteria overview below.
Review criteria
less 
When you submit your assignment, other learners in the course will review and grade your work. These are the criteria they’ll use to evaluate your APIs.

In this project, your APIs need to make it possible for your end-users to perform certain tasks and your reviewer will be looking for the following functionalities.

1.	The admin can assign users to the manager group

2.	You can access the manager group with an admin token

3.	The admin can add menu items 

4.	The admin can add categories

5.	Managers can log in 

6.	Managers can update the item of the day

7.	Managers can assign users to the delivery crew

8.	Managers can assign orders to the delivery crew

9.	The delivery crew can access orders assigned to them

10.	The delivery crew can update an order as delivered

11.	Customers can register

12.	Customers can log in using their username and password and get access tokens

13.	Customers can browse all categories 

14.	Customers can browse all the menu items at once

15.	Customers can browse menu items by category

16.	Customers can paginate menu items

17.	Customers can sort menu items by price

18.	Customers can add menu items to the cart

19.	Customers can access previously added items in the cart

20.	Customers can place orders

21.	Customers can browse their own orders

You'll also need to give feedback on and grade the assignments of two other learners using the same criteria.
Example Submissions
less 
Here are some examples to help you understand what your assignment should look like.

 Browsing menu-items endpoint using the browser:  

 How to create and submit your assignment
less 
You need to use pipenv to create the virtual environment and to manage the dependencies. Your APIs should be created using Django, DRF and Djoser. You need to use SQLite as the database for this project. You can develop your APIs using VS Code and test them using your browser or Insomnia. 

Name the project directory LittleLemon and the app LittleLemonAPI. Ensure that you follow this naming convention to make the reviewing process easier. 

You will be required to submit your APIs by uploading a zipped folder that contains your code. 

Important note: Include the sqlite database file db.sqlite3 in your project submission and share the superuser’s username and password of all the other users you have created. Write these usernames and passwords in a notes.txt file and keep it inside the project directory and then zip the project. 

To learn more about how to zip and unzip folders visit the 
Mac
 or 
Windows
 support page.            
How to review you peers
less 
Once you have submitted your file, you are required to review two peer submissions. You can view the peers that you need to review in the “Peers to review” section. You need to download their zipped project folder and unzip it. Then, prepare the virtual environment and install all dependencies using the following commands. 

cd LittleLemon

pipenv shell

pipenv install 

python manage.py makemigrations 

python manage.py migrate

python manage.py runserver

Then log into the Django admin panel and create superuser and user groups and randomly assign them into these groups, the same way you did in your own project. 
Examples of Good Feedback
less 
The focus of your feedback should be on the functionality of the APIs.

Follow the prompts and look for the expected output. If you notice any errors in the functionality of any of the elements of the APIs, you will have the opportunity to provide guidance to your peers on how they might fix the error. 

An example of good feedback would be:

“On the whole, the APIs performed as expected; however, customers couldn’t log in using their username and password and get access tokens. I would suggest reviewing the code you have written to ensure that the Djoser package was installed and configured correctly. You could revisit the video, 
Introduction to Djoser library for better authentication
 in Module 3, lesson 2.