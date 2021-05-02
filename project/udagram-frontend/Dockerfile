# Based on NodeJS 12
From node:12

# Create app directory in Docker
WORKDIR /usr/src/app

# Copy all files into the container
COPY . .

# Install projects node plugins
RUN npm install

# Instal ionic
RUN npm install -g ionic

# Build application
RUN ionic build

# Application available from this port
EXPOSE 8100

CMD ["ionic", "serve"]