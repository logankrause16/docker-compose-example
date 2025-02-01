# Use Python 3.9 or whichever version you want
FROM python:3.9-slim

# Set a working directory
WORKDIR /usr/src/app

# Copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY . .

# Expose port 8080 for Flask
EXPOSE 8080

# Run Flask (assuming your Flask app is in app.py)
CMD ["python", "app.py"]
