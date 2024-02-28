# Getting started with flask

These are the steps that will get you started with flask, just follow the steps and for more information you will be provided with altenative options:

1. Go to python.org and istall python if you hadn't installed it.
2. Make sure when installing python you tick the checkbox that says **ADD Python to PATH** and tap install now. You could also go to advanced options and check the checkbox that talks about environment variable
   ![image that has add path checkbox](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.ics.uci.edu%2F~pattis%2Fcommon%2Fhandouts%2Fpythoneclipsejava%2Fimages%2Fpython%2Fpythonsetup.jpg&f=1&nofb=1&ipt=c36665c00912451ebd97f73ccae7d2f00409c9600c8aa7f87b0a3b2ef99c0e83&ipo=images)
   ![python advanced image](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.easytweaks.com%2Fwp-content%2Fuploads%2F2022%2F01%2Fadd_python_path_windows_10.png&f=1&nofb=1&ipt=6d75f58a899fe4a3799036fdea4d5a9f8121ef673f627a7e1af96ca94066f561&ipo=images)
   
2. go to any CLI (cmd, powershell, git, etc) and type python --version to check if python is there in your path as environment variable, if not then you need to manually add python as an environment variable in your computer settings.
3. check if pip was correctly installed with python by typing any pip command like **pip freeze** or **pip --version**
4. make a directory in any desired folder by typing **mkdir directoryName** but replace directoryName with your own name e.g mkdir flaskWebApp
5. type **cd directoryName** where directoryName is the name of your directory
6. install the virtual environment package py typing **pip install virtualenv**
7. create a virtual environment by typing **python -m venv venvflask**. you can replace **venvflask** with your own virtual environment name
8. Once you have a virtual environment you need tp activate it by **.\venvflask\Scripts\activate**. note, **venvflask** is the name of your virtual environment, you can only name it what you named when creating the environment.
   - The display should appear from something like **C:\Users\Berry\FlaskWebApp>** to **(venvflask) C:\Users\Berry\FlaskWebApp>**.
9. you are now inside a virtual environment so you can install any packages. start with installing flask by **pip install flask**, type **pip freeze** to check packages inside your environment.
10. type **echo.>** **main.py** to create your main file.
11. Open your IDE and open the folder of your repository. When you have opened the folder in your IDE you should see a folder of your virtual environment and the hello.py file you have created. If you do not see a subfolder of you virtual environment, make sure you have done it right.
12. Tap on your main.py file and start writing code
    '''
    from flask import flask

    app = Flask(__name__)

    @app.route('/')
    def index():
       return "<h2>Hello Flask</h2>"
    '''
14. Few adjustments before running the code *in your CLI under your virtual environment*.
   - Type **set  FLASK_ENV=development** to set your application to development
   - Type **set FLASK_APP=main.py** to set the file to run which is your main file.
15. Type **flask run**  to run your application
16. Copy the link you which is **127.0.0.1:5000** or **localhost:5000** and paste it in your browser to see the message we have written in our code beforw. :)

This is just a start of a flask application.
   

1. Install Python
2. Make sure pip and python are set as environment variable and appear in cmd/any command line interface you might be using
3. Install your favourite IDE (VSCode is recommended)
4. Go to cmd and type *python --version*. Also type *pip freeze* to check if pip exists... if there are any errors then you need to make sure python is correctly intalled with pip.
5. Install a virtual environment module by typing *pip install venv*
6. 
7. Clear your cmd and type *pip install flask*
8. After intalling flask 
