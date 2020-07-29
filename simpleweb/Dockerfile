# Build this with docker build -t jackmckew/simpleweb .
# Run this with docker run -p 8000:8000 jackmckew/simpleweb

# Specify a base image
FROM node:alpine

# Set working directory
WORKDIR /usr/app

# Mount package.json - do this to not have to install depedancies if other files change
COPY ./package.json ./

# Install dependencies
RUN npm install 

# Mount remaining files
COPY ./ ./

# Default command
CMD ["npm","start"]