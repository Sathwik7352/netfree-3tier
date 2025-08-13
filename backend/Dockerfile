FROM node:22

# Set working directory
WORKDIR /app

# Install dependencies first
COPY package*.json ./
RUN npm install

# Copy backend source code
COPY . .

# Expose backend port
EXPOSE 3000

# Run backend
CMD ["node", "index.js"]
