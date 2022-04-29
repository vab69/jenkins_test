# Использовать официальную среду исполнения Python в качестве родительского образа
FROM python:2.7-slim

# Установить рабочий каталог в /app
WORKDIR /app

# Скопируйте содержимое текущего каталога в контейнер в /app
COPY . /app

# Установите все необходимые пакеты, 
# указанные в файле requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Сделать порт 80 доступным 
# для мира за пределами этого контейнера
EXPOSE 80

# Определить переменную среды
ENV NAME World

# Запустить app.py при запуске контейнера
CMD ["python", "app.py"]