FROM httpd:latest

CMD ["httpd-foreground"]
CMD ["bash"]

EXPOSE 80

RUN apt-get update

ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in /


COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/
STOPSIGNAL SIGWINCH

ENV HTTPD_PATCHES=
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
ENV HTTPD_PREFIX=/usr/local/apache2
HTTPD_SHA256=20e01d81fecf077690a4439e3969a9b22a09a8d43c525356e863407741b838f4
ENV HTTPD_VERSION=2.4.51

WORKDIR /usr/local/apache2

