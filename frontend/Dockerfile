FROM node:latest

# Create and set the working directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./
RUN npm install

# Bundle app source
COPY . .

# Build the Next.js app
RUN npm run build

# Command to run your app
CMD ["npm", "start"]
