FROM node:24-alpine3.22 AS build
WORKDIR /app
COPY package* .
RUN npm install
COPY . .
ENV PORT=3000
ENV ENTRIES_SERVICE_ADDR="assa"
ENV OPENAI_API_KEY="assa"
ENV OPENAI_MODEL="assa"
EXPOSE 5000
CMD ["node", "index.js"]