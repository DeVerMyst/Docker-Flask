cd /path/to/python-docker
pip install Flask
pip freeze | grep Flask >> requirements.txt
touch app.py

export FLASK_APP=app.py
python3 -m flask run

docker build -t fl .   
docker images
docker run fl

ATTENTION AUX VERSIONS 
pip uninstall  Flask Jinja2
pip install Flask Jinja2
pip install shinx --upgrade
pip install ruamel.yaml --upgrade

RUN 
docker run fl  
marche pas 
curl localhost:5000

docker run --publish 8000:5000 fl

curl localhost:8000

http://localhost:8000