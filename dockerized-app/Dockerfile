# Step 1: Use an official Node.js image from Docker Hub
FROM node:16

# Step 2: Set the working directory inside the container
WORKDIR /usr/src/app

# Step 3: Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Step 4: Install the project dependencies
RUN npm install

# Step 5: Copy the rest of the application files to the container
COPY . .

# Step 6: Expose port 3000 (or any port your app uses)
EXPOSE 3000

# Step 7: Command to run the app when the container starts
CMD ["node", "app.js"]