FROM python:3.10-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

# Expose the dev backend port
EXPOSE 3001

# Use environment variables from .env file (handled by docker-compose)
CMD ["python", "app.py"]