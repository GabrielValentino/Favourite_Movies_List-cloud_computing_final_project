#We use an official node image
FROM node:latest
#We specify the xorking directory
WORKDIR /app
#We copy all of the current directory in the container (our frontend code and dependencies)
COPY . .
#We install the dependencies.
#We will among other things install the 2 .json packages that are in the directory : 
# package.json and package-lock.json
RUN npm install
#We expose the port 3000(default port of our application)
EXPOSE 3000
#And then we start our backend container
CMD ["npm", "start"]