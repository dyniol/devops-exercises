FROM python:3.6.9
ENV FLASK_APP app/main.py
ENV FLASK_RUN_HOST 0.0.0.0

COPY . /home/dakar/coding/devops/exercises/flask_container_ci/challenge_venv/
# RUN apk add --no-cache gcc musl-dev linux-headers
WORKDIR /home/dakar/coding/devops/exercises/flask_container_ci/challenge_venv/
# COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
# COPY . .
EXPOSE 5000

CMD [ "flask", "run"]