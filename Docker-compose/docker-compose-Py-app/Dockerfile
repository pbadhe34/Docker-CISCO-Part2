# Use an official Python runtime as a parent image
FROM python:2.7-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt 
#ADD requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt 

# Make port 8090 available to the world outside this container
EXPOSE 8090

# Define environment variable
ENV NAME WebUser

# Run app.py when the container launches
CMD ["python", "app.py"]