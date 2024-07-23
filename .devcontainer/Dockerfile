FROM golang:1.22.5-bookworm

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        fish \
        git \
        openssh-client \
        sudo

# # Setup user
# RUN adduser $USERNAME -s /bin/sh -D -u $USER_UID $USER_GID && \
    # mkdir -p /etc/sudoers.d && \
    # echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME && \
    # chmod 0440 /etc/sudoers.d/$USERNAME

# Install packages and Go language server
#RUN go get -u -v golang.org/x/tools/cmd/gopls 2>&1