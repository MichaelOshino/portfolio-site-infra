FROM almir/webhook:latest
ARG UID=999
ARG USER=webhookcustom
USER root
RUN apk add --no-cache openssh-client && \
    addgroup -g ${UID} ${USER} && \
    adduser -u ${UID} -G ${USER} -D ${USER}
USER nobody