FROM python:3.11-slim

WORKDIR /app

# Installer dépendances système nécessaires
RUN apt-get update && apt-get install -y build-essential gcc git && rm -rf /var/lib/apt/lists/*

# Copier requirements et installer
COPY ./requirements.txt /app/requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Copier le reste du backend
COPY . /app

# Exposer le port (Railway fournira $PORT)
EXPOSE 8001

# Lancer uvicorn en utilisant la variable d'environnement PORT si fournie par la plateforme
CMD ["sh", "-c", "uvicorn server:app --host 0.0.0.0 --port ${PORT:-8001}"]
