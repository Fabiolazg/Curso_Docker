FROM python:3

# Instalação correta para Python 3:
# 'python3-pip' substitui 'python-pip'
# 'python3-dev' (ou 'python-dev-is-python3') substitui 'python-dev'
RUN apt-get update -y && \
    apt-get install -y python3-pip python3-dev 

WORKDIR /app

RUN pip install Flask requests flask_mysqldb

COPY . .

EXPOSE 5000

CMD ["python", "./app.py"]