# Use slim Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy files from the analytics folder to /app
COPY analytics/ /app/

# Install required Python packages
RUN pip install --no-cache-dir -r requirements.txt

# Command to run the app
CMD ["python", "app.py"]
