#Especifica imagem base
From node:14.17.5
#criar diretório de trabalho
WORKDIR /app
#copiando arquivos que possuiem os pacotes a ser utilizados
COPY package*.json ./
RUN npm install
#copia o restante dos arquivos
COPY . .
#expor a porta onde o serviço vai rodar
EXPOSE 8080
#comando de incialização do container
CMD ["node","server.js"]