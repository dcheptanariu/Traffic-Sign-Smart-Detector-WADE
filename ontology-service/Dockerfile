# Use the official Python image
FROM python:3.9-slim

RUN apt-get update
# Set the working directory
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application files
COPY . .

# Expose the port Flask runs on
EXPOSE 8080


# Set the default command to run the application
CMD ["python", "main.py"]
