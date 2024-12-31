# Use an official Python slim runtime as a parent image
FROM python:3.11-slim

# Set the working directory
WORKDIR /helloworld

# Install dependencies
COPY requirements.txt /helloworld/
RUN pip install -r requirements.txt

# Copy the project code into the container
COPY . /helloworld/

# Expose the port
EXPOSE 8000

# Command to run the code on port 8000
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]