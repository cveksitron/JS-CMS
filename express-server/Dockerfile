# Docker Parent Image with Node and Typescript
FROM node

# Create Directory for the Container
WORKDIR /express-server

# Copy the files we need to our new Directory
ADD . /express-server

# Grab dependencies and transpile src directory to dist
RUN npm install -g typescript
RUN npm install && tsc

# Expose the port outside of the container
EXPOSE 3000

# Start the express-server
CMD ["npm", "start"]