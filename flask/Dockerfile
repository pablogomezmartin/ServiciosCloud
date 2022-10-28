FROM python:3.8-slim-buster

WORKDIR /app

#Copiar requirements.txt en el directorio , es análogo a hacer el COPY . . 
COPY  requirements.txt requirements.txt 
RUN pip3 install -r requirements.txt

#Copiar el código fuente de la aplicación
COPY . .

#Exponemos el puerto en el que se va a ejecutar
EXPOSE 5000

#Indicamos el comando que tiene que ejecutar el contenedor
CMD ["python3","-m","flask","run", "--host=0.0.0.0"]
