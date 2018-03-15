# flask-celery-periodic-task
A simple Flask app to demonstrate Celery periodic task. 

## Requirements:
* Python 2.7
* Redis Server
## Running:
1. Start the Redis server: `redis-server` 
2. start the celery beat service: `celery -A app.celery beat`
3. Start the Celery worker: `celery -A app.celery worker --loglevel=info`
4. Run the Flask app:
```
export FLASK_APP=app.py
flask run
```

