# Pull the Node.js Docker image
FROM node:alpine

# Create the directory /usr/src/app inside the container
WORKDIR /usr/src/app

# Copy the package.json files from local machine to the workdir in the container
COPY package*.json ./

# Run npm install in our local machine
RUN npm install

# Copy all the files in the directory from local machine to the working directory (including node_modules)
COPY . .

# We need to expose port 5000, which is running within the container, to view it on our browser
EXPOSE 5000

# Command to run when the container is started.
CMD ["node", "index.js"]