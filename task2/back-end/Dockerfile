# Étape 1 : utiliser Ubuntu latest
FROM ubuntu:latest

# Étape 2 : mettre à jour et upgrader
RUN apt-get update && apt-get upgrade -y

# Étape 3 : installer Python3 et pip3
RUN apt-get install -y python3 python3-pip

# Étape 4 : supprimer le fichier EXTERNALLY-MANAGED si nécessaire
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Étape 5 : installer Flask avec pip3
RUN pip3 install flask

# Étape 6 : définir le dossier de travail
WORKDIR /app

# Étape 7 : copier ton script dans l’image
COPY ./api.py /app/api.py

# Étape 8 : lancer le serveur Flask
CMD ["python3", "api.py"]
