FROM alpine:latest
RUN apk add --no-cache curl bash net-tools
RUN curl https://storage.yandexcloud.net/yandexcloud-yc/install.sh | bash
ENV PATH="/root/yandex-cloud/bin:${PATH}"
RUN curl -sL "https://github.com/warrensbox/terraform-switcher/releases/download/0.13.1308/terraform-switcher_0.13.1308_linux_amd64.tar.gz" | tar -xzv -C /usr/local/bin tfswitch
RUN curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh && rm get-docker.sh

