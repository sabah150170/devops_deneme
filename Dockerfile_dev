# Node.js image
FROM node:14-alpine

# Set working directory
WORKDIR /app/Node_API

# Copy the file of the application code
COPY . .

# Install application dependencies
RUN rm -f yarn.lock
RUN npm install

# Define environment variable
ENV PORT 9090
ENV NODE_ENV production
ENV DB_USER prod_user
ENV DATABASE_PASSWORD prod_pw
ENV DB_HOST 172.17.0.6
ENV DB_PORT 5432
ENV DB_DATABASE foodie
ENV DATABASE_URL postgresql://prod_user:prod_wd@172.17.0.6:5432/foodie

# Run the application
CMD ["node", "server.js"]
