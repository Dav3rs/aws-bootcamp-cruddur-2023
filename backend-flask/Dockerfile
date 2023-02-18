FROM python:3.10-slim-buster

WORKDIR /backend-flask

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

ENV FLASK_ENV=development
ENV FRONTEND_URL="*"
ENV BACKEND_URL="*"

EXPOSE 4567

CMD [ "python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=4567" ]