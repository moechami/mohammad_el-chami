FROM mcr.microsoft.com/devcontainers/universal:2-linux

# Update and install system dependencies
RUN apt-get update && apt-get install -y \
    python3-pip \
    nodejs \
    npm \
    && rm -rf /var/lib/apt/lists/*

# Install Python dependencies
RUN pip install Flask

# Set up working directory
WORKDIR /app

# Install Vue CLI globally
RUN npm install -g @vue/cli
