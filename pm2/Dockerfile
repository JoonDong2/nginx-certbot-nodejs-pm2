FROM keymetrics/pm2:12-alpine

# Bundle APP files
COPY pm2/src src/
COPY pm2/package.json .
COPY pm2/pm2.json .

# Install app dependencies
ENV NPM_CONFIG_LOGLEVEL warn
RUN npm install --production

# Show current folder structure in logs
RUN ls -al -R

CMD [ "pm2-runtime", "start", "pm2.json" ]