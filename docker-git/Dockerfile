FROM ubuntu:22.04
RUN apt-get update && apt-get install --yes --no-install-recommends git make
LABEL description="Une image contenant git préconfiguré"
RUN git config --global init.defaultBranch ma_grosse_branche