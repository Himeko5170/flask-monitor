# FLASK MONITORING
### powered by baso-03-17

## RUN
```
git clone https://github.com/himeko5170/flask-monitor.git
cd flask-auth
python3 -m venv venv
. venv/bin/activate
pip install -r requirements.txt
python
>>> from server import db, create_app
>>> db.create_all(app=create_app())
>>> exit
cp .env.bak .env
cd server/
python3 -m flask run
```

## RUN ON HTTPS
```
sudo apt-get install openssl
openssl req -x509 -newkey rsa:4096 -nodes -out cert.pem -keyout key.pem -days 365
python3 -m flask run --cert=cert.pem --key=key.pem 
```
