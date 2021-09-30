# deployer-sur-Heroku
Ici est une partie d'un tuto sur youtube ou je vous montre comment deployer un project django en moins de 15 minites.

1-CREER VOTRE DJANGO</br> 
Assurez vous que l'environnemetn virtual est active si vous en avez.

2-INSTALLER psycopy2, gunicorn, django-heroku</br> 

3-CREER LE FICHIER runtime.txt</br> 

4-CREER LE FICHIER Procfile sans extension</br> 

5-GENERER Le fichier requirements.txt
Rassenble tout vous pakage dans le fichier requirements.txt grace a la commade suivanate.
pip freeze > requirements.txt</br>


6-METTRE TON PROJECT SUR GIT

INSTALLER GIT 
https://www.atlassian.com/git/tutorials/install-git

                                                                                     

--CREER UN CONPTE SUR HEROKU  </br>                                                                                                   
https://signup.heroku.com/</br>

--DOWNLOAD HEROKU CLI</br>
https://devcenter.heroku.com/articles/heroku-cli</br>

--CONFIGURER DJANGO HEROKU</br>
https://devcenter.heroku.com/articles/django-app-configuration</br>

POUR AVOIR LA CONFIGURATION DU WHITENOISE 
https://whitenoise.evans.io/en/stable/django.html

DANS LE TERMINAL TAPEZ CES COMMANDES:</br>
git init</br>
git add .</br>
git commint -m "premier commit"</br>
heroku login </br>
heroku create nom_du_domain</br>
git push heroku master</br>
heroku run python manage.py migrate</br>
heroku open</br>

dans le setting DEBUG=False</br>

si vous faite des modification sur votre application la seul chose a faire c'est de taper ces lignes de commande:</br>
git init</br>
git add .</br>
git commint -m "expliquer en un ou deux mots la modification ici"</br>
git push heroku master
