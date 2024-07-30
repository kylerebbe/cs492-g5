## Kyles Installation notes <br>
For windows: <br>
1. Install VS CODE <br>
2. Install Git <br>
3. Install Python 3.12 <br>
4. Install pip (https://pypi.org/project/pip/) <br>
 <br>
5. Add python to environment variable path  <br>
` C:\Users\kyler\AppData\Local\Programs\Python\Python312 ` <br>
6. Add python scripts folder to environment path 
`C:\Users\kyler\AppData\Local\Programs\Python\Python312\Scripts` <br>

7. Open App Execution Aliases windows settings : <br>
	* Disable App Installer: python.exe <br>
	* Disable App Installer: python3.exe <br>

8. Git Clone Group Project Repository (https://github.com/kylerebbe/cs492-g5)
 	* Add ssh key to github profile (https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) <br>
 
9. In VS Code, select python interpreter: <br>
	* ctrl + shift + p > Python Select interpreter <br> `Set to python 3.12` <br>

10. Install Python Virtual Environment Manager <br>
11. Create Virtual Environment in workspace. (.venv) <br>

12. Click the "open in terminal" button under Workspace environments > .venv(3.12.4) <br>	-Note : you may need to enable script execution in power shell if that is your default terminal.
	* Open a power shell as administrator from start menu and type in the following command:  `Set-ExecutionPolicy RemoteSigned`
	
13. From the vs code terminal type the following to ensure your project venv is up to date.  You only need to run this if dependencies in "requirements.txt" change.<br>
`pip install --ignore-installed -r .\requirements.txt`

#### 14. To run application/website, type in the following from the terminal with vertual environment activated: <br>
`py .\manage.py runserver`

#### 15. Open website browser and navigate to `127.0.0.1:8000`


## Original Installation Notes

1. Open terminal using Ctrl+T. Run the following command <br>
`git clone https://github.com/HemabhKamboj/Pizza-ordering-app.git`

2. Create and active virtual environment using  <br>
` virtualenv -p python3 venv` <br>
` cd venv` <br>
`source bin/activate` <br>
3. Change the directory using <br>
`cd ..` <br>
` cd Pizza-ordering-app master`
4. Now you need to install python packages to run the app <br>
`pip3 install -r requiements.txt`
5. Create superuser <br>
 `python manage.py createsuper`
6. Run Django app <br>
`python manage.py runserver`

## Tech Stack

- **Django**  Django is a Python-based free and open-source web framework,
 which follows the model-view-template architectural pattern. It is maintained by the Django Software
 Foundation, an independent organization established as a 501 non-profit. 
Django's primary goal is to ease the creation of complex, database-driven websites. [Django Project](https://www.djangoproject.com/) <br>
It is used in this project, to handle all routes, rendering pages, managing databases, 
user authentication and almost all the stuff of which the application is capable of.
- **SQLite** SQLite is a relational database management system contained in a C programming library. In contrast to many other database management systems, 
SQLite is not a client–server database engine. Rather, it is embedded into the end program<br>
It comes with Django with itself, no setup required, hence easy to use, but is not recommended for large scale
production application.
- **Bootstrap** Bootstrap is a free and open-source front-end Web framework. It contains HTML and CSS-based design templates for typography, forms, buttons, navigation and other
 interface components as well as optional JavaScript extensions. [Get Bootstrap](getbootstrap.com) <br>
Used for stylising frontend. 
