# Use the official Node.js 20 image as the base image
# This includes Node.js and npm pre-installed
FROM node:20

# Set the working directory inside the container to /app
# All subsequent commands will run from this directory
WORKDIR /app

# Copy package.json and package-lock.json (if present) into the container
# This helps Docker cache dependencies and avoid reinstalling them unless they change
COPY package*.json ./

# Install project dependencies defined in package.json
# This installs the necessary Node.js packages into the container
RUN npm install

# Copy the rest of the application code into the container
# This includes src/, config files, etc.
COPY . .

# Define the command to run your app when the container starts
# This launches the app using Node.js and the entry point file
CMD ["node", "./src/index.js"]
