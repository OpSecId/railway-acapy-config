FROM ghcr.io/openwallet-foundation/acapy-agent:py3.12-1.3.2

RUN pip install git+https://github.com/openwallet-foundation/acapy-plugins@1.3.2#subdirectory=webvh

COPY ./configs.yml configs.yml

CMD ["start", "--arg-file", "configs.yml"]
