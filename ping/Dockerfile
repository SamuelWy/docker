FROM quay.io/openshifttest/pod-for-ping
RUN sed -i 's/v3.5/v3.6/g' /etc/apk/repositories
RUN cat /etc/apk/repositories
RUN rm -rf /var/cache/apk
RUN mkdir /var/cache/apk
RUN apk update --allow-untrusted
RUN apk upgrade --available
RUN sync
RUN reboot
RUN cat /etc/alpine-release
RUN cat /etc/issue
