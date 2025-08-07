FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy only requirements
COPY analytics/requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the entire analytics app code
COPY analytics/ .

# Run the app
CMD ["python", "analytics/app.py"]

