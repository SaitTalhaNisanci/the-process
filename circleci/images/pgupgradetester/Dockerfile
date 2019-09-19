# FROM python:3.6-slim
FROM python@sha256:6411a78d12cd3bd1e594c3dd1532ed02e62da744bbc92863a7548ae2de9e7dfa

COPY files /tmp

RUN set -ex; \
	ln -s /tmp/sbin/* /usr/local/sbin/; \
	ln -s /tmp/bin/* /usr/local/bin; \
	install-testdeps

WORKDIR /home/circleci
