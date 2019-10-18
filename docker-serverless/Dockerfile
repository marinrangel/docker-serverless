# use this dockerfile to build an image for this api

FROM node:10

WORKDIR /usr/src/app

COPY package*.json ./

RUN yarn install && yarn global add serverless

EXPOSE 3000 49153

CMD [ "sls", "offline", "start" ]
# ENV AWS_ENDPOINT='http://localhost:8000'
# ENV AWS_REGION='us-west-1'
# ENV AWS_ACCESS_KEY_ID='from-dockerfile-fake-access-key'
# ENV AWS_SECRET_ACCESS_KEY='from-dockerfile-fake-secret-key'