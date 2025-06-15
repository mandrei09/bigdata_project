# Use official Python base image
FROM python:3.11-slim

# Set environment variables
ENV DEBIAN_FRONTEND=noninteractive
ENV JAVA_VERSION=17

# Install system dependencies and Java 17
RUN apt-get update && apt-get install -y --no-install-recommends \
    openjdk-17-jdk curl git bash && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Set JAVA_HOME manually
ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
ENV PATH="$JAVA_HOME/bin:$PATH"

# Install Python packages (PySpark includes Spark already)
RUN pip install --upgrade pip && \
    pip install pyspark jupyterlab ipykernel notebook && \
    pip install pandas matplotlib seaborn scikit-learn numpy

# Create workspace
WORKDIR /workspace

# Default command
CMD ["bash"]
