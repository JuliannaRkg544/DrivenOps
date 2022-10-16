FROM node:16

WORKDIR /app

COPY . . 

RUN npm i 
RUN npm run build

# precisamos de um servidor de arquivos (nginex)

RUN mkdir -p /var/www/html
RUN mv build/* /var/www/html

WORKDIR / 
RUN rm -rf /app