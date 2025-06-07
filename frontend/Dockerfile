# ✅ Updated Node.js version
FROM node:18.20-alpine

# Set working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy app source
COPY . .

# Build Next.js app
RUN npm run build

# Expose app port
EXPOSE 3000

# Start the app
CMD ["npm", "run", "start"]
