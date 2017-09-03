# скачать образ python версии 2.7
FROM python:2.7   

# создать директорию
RUN mkdir -p /code

# скопировать всё содержимое (Файлы requremants  И flaskapp) текущей директории, в котором находится Dockerfile в созданную директорию  
COPY .  /code   
     
# подключить
VOLUME [ "/code" ]   

# рабочим каталогом будет code
WORKDIR /code       

# pip -r requirements.txt – Проинсталировать зависимости для Python
RUN pip install -r requirements.txt 

EXPOSE 5000
CMD [ "python", "/code/flask.app" ]
