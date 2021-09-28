# deployer-sur-Heroku
Ici est une partie d'un tuto sur youtube ou je vous montre comment deployer un project django en moins de 15 minites.

INSTALLER GIT 
https://www.atlassian.com/git/tutorials/install-git

Assurez vous que l'environnemetn virtual est active si vous en avez.
Rassenble tout vous pakage dans le fichier requirements.txt grace a la commade suivanate.

pip freeze > requirements.txt

AJOUTER DANS LE FICHIER setting.py cette ligne

STATIC_ROOT = os.path(BASE_DIR, 'static')

--CREER UN CONPTE SUR HEROKU
https://signup.heroku.com/

--DOWNLOAD HEROKU CLI
https://devcenter.heroku.com/articles/heroku-cli

--CONFIGURER DJANGO HEROKU
https://devcenter.heroku.com/articles/django-app-configuration

DANS LE TERMINAL TAPEZ CES COMMANDES:
git init
git add .
git commint -m "premier commit"
heroku login 
heroku create nom_du_domain
git push heroku master
heroku run python manage.py migrate
heroku open

dans le setting DEBUG=False

si vous faite des modification sur votre application la seul chose a faire c'est de taper ces lignes de commande:
git init
git add .
git commint -m "expliquer en un ou deux mots la modification ici"
git push heroku master
