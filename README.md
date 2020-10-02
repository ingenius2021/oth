# the-pursuit

An OTH (Online Treasure Hunt) app based on Python/Django. It is forked from this project. It was used to host The Pursuit 2016 organised by PESITSouth ACM, that saw participation from over 400 users from 20+ countries.

# Features
Any number of questions can be added using a web-based GUI (Django admin), no coding required.
Uses randomly generated image names so users can't see other level images by guessing the URL.
User can only view the current level.
Supports three types of questions/hints - text, image and hidden text (HTML comment).
In-built support for login, registration and session management.
A leaderboard that takes both the level, and completed time into account.
Winners are separately indicated in the leaderboard.
A start page with rules, and a finish page for the users who complete the OTH.

# Instructions
Set up a virtual environment and switch to it. (Optional, but recommended.) Following command can be used with virtualenv and virtualenvwrapper installed.

python -m venv myvenv

Install dependencies using pip.

pip install -r requirements-dev.txt [for develeopment]

pip install -r requirements-prod.txt [for production]

Go to the projetc's directory on the terminal.
python manage.py makemigrations oth
python manage.py migrate oth

Create a super user using:
python manage.py createsuperuser <username>
  
 Run the server:
 python manage.py runserver
 
 Go to http://localhost:8000/admin to add questions
 
# Credits
Thanks to code-haven for the original project.

# Author
Built by Amjad Ali for inGenius 2016 on behalf of PESITSouth ACM.
 
 
