# CONTRIBUTING

## Virtual Env

```bash
python3.10 -m venv .venv
source .venv/bin/activate
```

## How to build the image

```bash
docker build -t pojan-flask-rest-api .   
```

## How to run the Dockerfile locally

```bash
docker run -p 5000:5000 -w /app -v "$(pwd):/app" pojan-flask-rest-api sh -c "flask run --host 0.0.0.0"
```

## How to locally install requirements.txt

```bash
pip install -r requirements.txt  
```

## DB Init

```bash
flask db init
```

## Migration

```bash
flask db migrate
flask db upgrade
```

## Deployment

- https://dashboard.render.com/
- https://api.elephantsql.com/
