# Use an official Node.js runtime as the base image
FROM node:latest

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Build the React app (replace 'npm run build' with your actual build command)
RUN npm run build

# Expose the port that the application will run on (typically 3000 for Create React App)
EXPOSE 3000

# Define the command to run the application
CMD ["npm", "start"]
