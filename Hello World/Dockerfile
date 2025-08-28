# use the official python image from the Docker Hub
FROM python:3.9-slim

# set the working directory
WORKDIR /app

# copy the requirements file
COPY . /app

# install the dependencies
RUN pip install flask

# copy the rest of the application code
COPY . .

# Make port 5000 available to the works outside this container
EXPOSE 5000

# set the command to run the application
CMD ["python", "app.py"]