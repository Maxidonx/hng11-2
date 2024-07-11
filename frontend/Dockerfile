# Use the latest official Node.js image as a base
FROM node:latest


RUN apt-get update && apt-get install -y \
    nodejs \
    npm

# Set the working directory
WORKDIR /app

# Copy the application files
COPY . .

# Install dependencies
RUN npm install

# Expose the port the development server runs on
EXPOSE 5173

# Run the development server
CMD ["npm", "run", "dev", "--", "--host"]