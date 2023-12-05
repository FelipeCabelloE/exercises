# Use Microsoft Planetary Computer's Python image as a parent image
FROM mcr.microsoft.com/planetary-computer/python:latest

# Set the working directory in the container to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
#RUN pip install --no-cache-dir -r requirements.txt

# Git configuration (replace with actual values or use build arguments)
ARG GIT_USER
RUN git config --global user.name "${GIT_USER}"
RUN git config --global user.email "${GIT_USER}@users.noreply.github.com"
