# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set environment variables
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install dependencies
RUN pip install --no-cache-dir Flask

# Expose port 5000
EXPOSE 5000

# Run the Flask application
CMD ["flask", "run"]
