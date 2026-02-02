FROM node:24-alpine3.22
WORKDIR /app
COPY services/api-gateway/package* .
RUN npm install
COPY services/api-gateway/. .
COPY protos ./protos
ENV PORT=5000
#ENV ENTRIES_SERVICE_ADDR="assa"
#ENV OPENAI_API_KEY="assa"
#ENV OPENAI_MODEL="assa"
EXPOSE 5000
CMD ["node", "index.js"]