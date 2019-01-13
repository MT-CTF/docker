FROM node:10

# Create app directory

RUN apt-get install -y git-core
RUN cd /tmp && git clone https://github.com/thomasrudin-mt/mail && mv /tmp/mail/webmail /webmail && rm -r /tmp/mail
WORKDIR /webmail
RUN ls
RUN npm install --only=production

EXPOSE 8080
CMD [ "node", "src/index.js" ]
