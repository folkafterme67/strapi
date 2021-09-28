FROM node:14
WORKDIR /usr/src/app
# #WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
# RUN ls -l
ENV NODE_ENV production
ENV DATABASE_CLIENT=mysql
ENV DATABASE_NAME=Skyller
ENV DATABASE_HOST=0.0.0.0
ENV DATABASE_PORT=3306
ENV DATABASE_USERNAME=root
ENV DATABASE_PASSWORD=
CMD ["npm", "start"]



# # EXPOSE 3002

# FROM node
# WORKDIR /build
# COPY package.json .
# RUN npm install
# COPY . .
# ENV NODE_ENV production
# ENV DATABASE_CLIENT=mysql
# ENV DATABASE_NAME=Skyller
# ENV DATABASE_HOST=0.0.0.0
# ENV DATABASE_PORT=3306
# ENV DATABASE_USERNAME=root
# ENV DATABASE_PASSWORD=
# RUN npm run build
# EXPOSE 1337
# CMD ["npm", "start"]