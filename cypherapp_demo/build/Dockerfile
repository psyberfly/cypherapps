# Step 1: Use a lightweight Node.js image
FROM node:alpine

# Step 2: Set the working directory
WORKDIR /app

# Step 3: Copy package.json and package-lock.json if using npm (or yarn.lock if using yarn)
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy your app's source code
COPY . .

# Step 6: Expose the development server port (default: 3000)
EXPOSE 5173

# Step 7: Start the development server
CMD ["npm", "start"]
