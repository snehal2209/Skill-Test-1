FROM python:3.10-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

# Expose the prod backend port
EXPOSE 3002

CMD ["python", "app.py"]