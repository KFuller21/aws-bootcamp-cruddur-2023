FROM python:3.10-slim-buster

# Inside Container
# Make a new folder inside container
WORKDIR /backend-flask

# Outside Container -> Inside Container
# This contains the libraries desired to run the App
COPY requirements.txt requirements.txt

# Inside Container
# Install the python libraries used for the App
RUN pip3 install -r requirements.txt

# Outside Container -> Inside Container
COPY . .

# Set environment variables for Inside Container (Env Vars)
ENV FLASK_ENV=development

EXPOSE ${PORT}

# Command = CMD
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]