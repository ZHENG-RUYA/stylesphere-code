
FROM python:3.9-slim
WORKDIR /app
COPY frontend/requirements.txt .
RUN pip install -r requirements.txt
COPY frontend .
CMD ["python", "app.py"]
EXPOSE 5000
