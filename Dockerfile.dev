FROM node:22-alpine as development

# Working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application code
COPY . .

# Start the application
CMD ["npm", "run", "start:dev"]