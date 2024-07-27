# Use an official image as a parent image
FROM --platform=linux/amd64 ubuntu:22.04

# Set the working directory
WORKDIR /workspace

# Install any dependencies
RUN apt-get update && apt-get install -y \
    curl \
    git \
    gcc \
    && rm -rf /var/lib/apt/lists/*

# Copy the current directory contents into the container at /workspace
COPY . /workspace

# Run any additional commands

# Expose port 3000
EXPOSE 3000

# Define the command to run the application
CMD ["bash"]
