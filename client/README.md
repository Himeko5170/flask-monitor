# FLASK MONITORING (AGENT)

## Pre-RUN
```
sudo apt-get install apache2
sudo systemctl enable apache2
sudo systemctl start apache2
```

## RUN
```
git clone https://github.com/rombintu/flask-monitor.git
cd flask-monitor/client
pip3 install psutil
python3 main.py
sudo ln info.json /var/www/html
настройте cron для автоматического обновления файла
```
