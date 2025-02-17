FROM python:3.9-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV FLASK_APP=app.py
ENV FLASK_ENV=development

EXPOSE 80

CMD ["python", "app.py"] 
# pour lancer python avec app.py



# CMD ["flask", "run", "--host=0.0.0.0", "--port=80"] pour faire un démarrage rapide flask run,