FROM python:3.11-slim

WORKDIR /app

# Copy project files
COPY . .

# Install dependencies
RUN pip install --no-cache-dir -r backend/requirements.txt

# Expose Flask port
EXPOSE 5000

# Environment variables
ENV FLASK_APP=backend/run.py
ENV PYTHONUNBUFFERED=1

# Start Flask application
CMD ["python", "backend/run.py"]