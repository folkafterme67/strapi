# FROM node:14-alpine
FROM strapi/strapi
WORKDIR /srv/app
# #WORKDIR /app
COPY package.json .
# COPY ./yarn.lock ./
RUN npm install --arch=x64 --platform=linux
#RUN yarn install
COPY . .
ENV NODE_ENV production
RUN npm run build
#RUN yarn build
EXPOSE 1337
CMD ["strapi", "start"]



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