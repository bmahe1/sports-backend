# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Expose port (Elastic Beanstalk will map process.env.PORT)
EXPOSE 8080

# Start the app
CMD ["node", "server.js"]
