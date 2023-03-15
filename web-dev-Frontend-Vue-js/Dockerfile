#We use an official node image
FROM node:latest
#we define our working directory
WORKDIR /app
#We copy all of the current directory in the container (our frontend code and dependencies)
COPY . .
#We install the dependencies
#We will among other things install the 2 .json packages thar are in the directory : 
# package.json and package-lock.json
RUN ["npm", "install"]
#we build the app
RUN ["npm", "run", "build"]
#And then we run the container
CMD ["npm", "run", "preview"]