# Use the official Python 3.7.5 image as the base image
FROM python:3.7.5

# Set the working directory in the container
WORKDIR /app

RUN apt-get update

# Copy the requirements file into the container
COPY requirements.txt .

# Install the necessary Python packages
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Expose the port that Pyplan IDE will run on (default 8080, change if necessary)
EXPOSE 9740

# Run the Pyplan IDE with django port
# CMD ["pyplan", "--host=0.0.0.0", "--port=9740"]