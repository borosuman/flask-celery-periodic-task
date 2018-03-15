# flask-celery-periodic-task
A simple Flask app to demonstrate Celery periodic task. 

## Requirements:
* Python 2.7
* Redis Server
## Running:
1. Start the Redis server: `redis-server` 
2. Start the Celery worker: `celery -A app.celery worker --loglevel=info`
3. Run the Flask app:
```
export FLASK_APP=app.py
flask run
```

