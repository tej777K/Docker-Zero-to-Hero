FROM python:3.8-slim

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN pip install -r requirements.txt && \
    cd devops

ENTRYPOINT ["python"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
