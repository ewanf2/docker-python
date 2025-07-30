FROM python:3.11-slim
WORKDIR /app

ENV PYTHONPATH=/app
ENV FLASK_APP=app.py

RUN apt-get update && apt-get install -y --no-install-recommends build-essential default-libmysqlclient-dev pkg-config

COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 5000
COPY .. .
CMD ["python", "app.py"]
