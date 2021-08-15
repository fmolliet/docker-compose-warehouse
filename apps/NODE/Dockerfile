FROM node:12-slim

# Create an app directory in the docker
WORKDIR /app

# Copy the package.json and package-lock.json. 
COPY package*.json ./

# Install production dependencies.
RUN npm install --only=production

# Copy local code to the container image.
COPY . ./

ENV PORT 8080
ENV HOST 0.0.0.0
ENV BASEURL https://test.api

EXPOSE 8080
# Run the server
CMD node src/server.js