FROM ghcr.io/openwallet-foundation/acapy-agent:py3.12-1.3.2

USER root

RUN pip install git+https://github.com/openwallet-foundation/acapy-plugins@1.3.2#subdirectory=firebase_push_notifications

USER $user
COPY ./configs.yml configs.yml

CMD ["start", "--arg-file", "configs.yml"]
