FROM node

RUN mkdir -p /usr/cr-app/frontend
WORKDIR /usr/cr-app/frontend
COPY package.json /usr/cr-app/frontend
COPY yarn.lock /usr/cr-app/frontend

RUN yarn install

COPY . /usr/cr-app/frontend

CMD ['yarn', 'start']