FROM python:3.9-slim-buster
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5001
ENV FLASK_APP=run.py
CMD ["flask", "run", "--host", "0.0.0.0"]