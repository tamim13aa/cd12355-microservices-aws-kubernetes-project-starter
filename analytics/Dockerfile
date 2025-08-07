# Use official lightweight Python image
FROM python:3.9-slim

# Set working directory in the container
WORKDIR /app

# Copy only requirements first to leverage Docker cache
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the entire analytics code
COPY . .

# Run the app
CMD ["python", "app.py"]
