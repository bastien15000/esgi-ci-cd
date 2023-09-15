FROM node:19
RUN apt-get update \
  && apt-get install -y --no-install-recommends \
  && curl -sSL https://github.com/hadolint/hadolint/releases/download/v2.12.0/hadolint-Linux-x86_64 -o /usr/local/bin/hadolint \
  && chmod a+x /usr/local/bin/hadolint \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
WORKDIR /app
COPY ./ /app
RUN npm install
