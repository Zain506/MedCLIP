# Use an official Python image as base
FROM python:3.11-slim
RUN apt-get update && apt-get install -y git
# Set working directory inside the container
WORKDIR /workspaces/MedCLIP

# Copy requirements.txt first (for caching)
COPY requirements.txt ./

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of your code (optional, Codespaces mounts your repo anyway)
# COPY . .

# Default command
CMD ["sleep", "infinity"]
