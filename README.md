# Understanding & Building Simple Application in Flask

![Header](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/flask_header.png)

## What is Flask?  
Flask is a micro web framework written in Python. 

It is classified as a microframework because it does not require particular tools or libraries. It has pros and cons. Pros would be that the framework is light, there are little dependency to update and watch for security bugs, cons is that some time you will have to do more work by yourself or increase yourself the list of dependencies by adding plugins. 

Its dependencies are:

* Werkzeug a WSGI utility library
* Jinja2 which is its template engine

### WSGI 
The Web Server Gateway Interface is a simple calling convention for web servers to forward requests to web applications or frameworks written in the Python programming language.

### Jinja2
Jinja is a web template engine for the Python programming language. It was created by Armin Ronacher and is licensed under a BSD License. Jinja is similar to the Django template engine but provides Python-like expressions while ensuring that the templates are evaluated in a sandbox. It is a text-based template language and thus can be used to generate any markup as well as source code.

Applications that use the Flask framework include Pinterest and LinkedIn.

## I have created a simple application using flask. Here is the step by step approach:

### Installation of Flask  

**Step-1: Installation of Python**  

Install latest version of [Python](https://www.python.org/downloads/release/python-390/)

**Step-2: Creation of directory and creation and activation of virtual environment**  
Type the following commands in Command Prompt:  

![Step-1-1](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/Step1-1.png)

The command `py -3 -m venv venv` is for virtual environment creation and `venv\Scripts\activate` will activate the virtual environment.

**Step-3 Installation of Flask**  
Then type `pip install flask` to install flask

![Step-1-3](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/Step1-3.png)

**Step-4: Creation of application using text editor**  
Although you can use any text editor, but I have used [Visual Studio Code](https://code.visualstudio.com/)

![flask-app](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/flask-app.png)

Note that, I have save this file in the same directory with the name [flask-app.py](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/flask-app.py)

**Step-5: Set the FLASK_APP and run the flask**  
Now to get the output type the command `set FLASK_APP=flask-app.py` and then `flask run` in the command prompt as shown:

![Step1-2](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/Step-1-2.png)

The important part here is `Running on http://127.0.0.1:5000/`
Just open the browser and type this `http://127.0.0.1:5000/` address

![hello-world](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/hello-world.png)
Congrats! You made a website with Flask!

### More fun with flask
Let’s make our website look nicer by adding HTML.

### HTML and Virtual Environments
**HTML and Templates in Flask**  

**Step-1:**

First create a new HTML file and name it as [home.html](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/home.html) and [about.html](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/about.html) Here is the code:

![home](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/home.png)

![about](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/about.png)

Now create a [flask1-app.py](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/flask1-app.py) file with the following code:

![flask1-app](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/flask1-app.png)

**Important Point To Remember**  
The Flask Framework looks for HTML files in a folder called **templates**. You need to create a templates folder and put all your HTML files in there and remember to always keep the **flask1-app.py** outside of your templates folder.

Now to get the output type the command `set FLASK_APP=flask1-app.py` and then `flask run` in the command prompt and type `http://127.0.0.1:5000/` address in browser, you will get

![home-browser](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/home-browser.png)

Than just type and `http://127.0.0.1:5000/about` in address bar, you will get 

![about-browser](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/about-browser.png)

**Step-2:**

Let’s Connect Both Pages with a Navigation
To connect both pages we can have a navigation menu on the top. We can use Flask to make the process of creating a navigation menu easier.

First, let’s create a [template.html](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/template.html). This **template.html** will serve as a parent template. Our two child templates will inherit code from it.

![template-navigation](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/template.png)

Content of **home.html**

![home-navigation](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/home-navigation.png)

Content of **about.html**

![about-navigation](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/about-navigation.png)

Now to get the output type the command `set FLASK_APP=flask1-app.py` and then `flask run` in the command prompt and type `http://127.0.0.1:5000/` address in browser, you will get

![navigation](https://github.com/shalakasaraogi/simple-application-in-flask/blob/main/images/navigation-browser.png)

You can find all the code file in this repository.



