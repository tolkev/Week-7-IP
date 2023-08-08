# Pull the Node image from Docker Hub
FROM node:18.15.0-alpine

# Setting Working Directory
WORKDIR /app

# Copying only package.json
COPY package*.json /app/

# Install Dependencies
RUN npm i

# Copy rest of the code to container
COPY . /app/

# Run the API on Nodemon
CMD ["npm", "start"]