# Use official Node.js image
FROM node:16

# Create app directory
WORKDIR /usr/src/app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Bundle app source
COPY . .

# Create uploads directory
RUN mkdir -p Uploads

# Expose the app port
EXPOSE 3002

# Start the application
CMD [ "node", "server.js" ]
