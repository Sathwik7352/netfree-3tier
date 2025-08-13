FROM node:22

# Set working directory
WORKDIR /app

# Install dependencies first
COPY package*.json ./
RUN npm install

# Copy frontend source code
COPY . .

# Expose frontend port (Vite default is 5173)
EXPOSE 5173

# Start frontend in dev mode
CMD ["npm", "run", "dev", "--", "--host"]
