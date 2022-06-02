#pull official base image
FROM python:3.10.4-slim-buster

# set work directory
WORKDIR /usr/src/app

# install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install -r requirements.txt

# # copy entrypoint.sh
# COPY ./entrypoint.sh .
# RUN sed -i "s/\r$//g" /usr/src/app/entrypoint.sh
# RUN chmod +x /usr/src/app/entrypoint.sh

# copy project
COPY . .
