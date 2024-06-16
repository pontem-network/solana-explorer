FROM node as build
WORKDIR /opt/app
RUN npm install -g pnpm
COPY . .
RUN pnpm fetch
RUN pnpm install
RUN pnpm run build
CMD ["pnpm", "start"]
