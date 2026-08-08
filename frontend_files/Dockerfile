
# Use a minimal base image with Python 3.9 installed
FROM python:3.9-slim

# Set the working directory inside the container to /app
WORKDIR /app

# Copy the frontend deployment artifacts into the container
COPY . .

# Install Python dependencies listed in requirements.txt
RUN pip3 install -r requirements.txt

# Run the Streamlit frontend on port 7860
CMD ["streamlit", "run", "bank_churn_frontend.py", "--server.port=7860", "--server.address=0.0.0.0"]
