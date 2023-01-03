#Base image
FROM node:16-alpine

#setting working directory
WORKDIR /app/frontend/

#copying package.json and package-lock.json files to working directory
COPY package*.json /app/frontend

#install all dependencies
RUN npm install

#copying our code content to the working directorys
COPY . /app/frontend

#server starting command
CMD ["npm", "start"]