FROM python:3.7
WORKDIR /app
COPY requirements.txt . 
RUN pip install --no-cache-dir --upgrade -r requirements.txt
COPY app.py .
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8080", "--no-server-header"]