FROM node:14
WORKDIR ./ohana-sai
COPY package.json ./
COPY package-lock.json ./
COPY . .
# Install production dependencies
RUN npm run setup-production

# Copy the rest of your app's source code
COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Start the app
CMD ["node", "server"]
