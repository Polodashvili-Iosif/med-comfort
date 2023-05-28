FROM python:3.7-slim

WORKDIR /app

COPY med_comfort .

RUN pip3 install -r requirements.txt --no-cache-dir

CMD ["gunicorn", "med_comfort.wsgi:application", "--bind", "0:8000"]