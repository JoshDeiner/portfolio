# Step 1: Build the React application
FROM node:18-alpine

ENV NODE_ENV=development

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json (or yarn.lock) files
COPY package*.json ./

# Install dependencies
RUN npm install --silent

# Copy the rest of your app's source code from your host to your app directory
COPY . .

EXPOSE 3000

# Run the application using the npm start script which should run react-scripts start
CMD ["npm", "start"]
