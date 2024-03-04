FROM oven/bun
WORKDIR /app
COPY bun.lockb .
COPY package.json .
RUN bun install --frezen-lockfile
COPY src ./src
EXPOSE 8080
CMD ["bun", "src/index.ts"]
