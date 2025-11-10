FROM ghcr.io/openwallet-foundation/acapy-agent:py3.12-1.4.0rc1

USER root

RUN pip install git+https://github.com/openwallet-foundation/acapy-plugins@1.3.2#subdirectory=webvh

USER $user
COPY ./config.yml config.yml

CMD ["start", "--arg-file", "config.yml"]
