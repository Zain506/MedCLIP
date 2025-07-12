# Use an official Python image as base
FROM python:3.11-slim

# Set working directory inside the container
WORKDIR /workspace

# Copy requirements.txt first (for caching)
COPY requirements.txt ./

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of your code (optional, Codespaces mounts your repo anyway)
# COPY . .

# Default command
CMD ["sleep", "infinity"]
