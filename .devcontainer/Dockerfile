FROM mcr.microsoft.com/devcontainers/python:3.10

# Install ffmpeg
RUN apt-get update && apt-get install -y ffmpeg && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Install spaCy + English model
RUN pip install --no-cache-dir spacy && \
    python -m spacy download en_core_web_sm
