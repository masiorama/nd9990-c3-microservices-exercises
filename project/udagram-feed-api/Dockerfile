# Based on NodeJS 12
From node:12

# Create app directory in Docker
WORKDIR /usr/src/app

# Copy all files into the container

COPY package*.json ./
RUN npm ci
COPY . .

# Application available from this port
EXPOSE 8080

CMD ["npm", "run", "dev"]