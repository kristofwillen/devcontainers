FROM python:3.12-slim

WORKDIR /code

RUN apt update
RUN apt -y install vim fish git

COPY ./src ./src

COPY ./requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

CMD [ "jupyter", "notebook", "--allow-root" ]
