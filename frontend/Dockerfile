#Base image
FROM node:17-alpine

#setting working directory
WORKDIR /app/frontend/

#copying package.json and package-lock.json files to working directory
COPY package*.json /app/frontend

#install all dependencies
RUN npm install

#copying our code content to the working directorys
COPY . /app/frontend

EXPOSE 3000

#server starting command
CMD ["npm", "start"]