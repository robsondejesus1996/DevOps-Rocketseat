# Usar uma imagem base do Node.js
FROM node:20-slim

# Definir o diretório de trabalho no contêiner
WORKDIR /usr/src/app

# Copiar o arquivo package.json e package-lock.json para o contêiner
COPY package*.json ./

# Instalar as dependências do projeto
RUN npm install

# Copiar o restante do código da aplicação para o diretório de trabalho
COPY . .

# Expor a porta que o servidor está escutando
EXPOSE 3000

# Definir o comando para iniciar a aplicação
CMD ["npm", "start"]
