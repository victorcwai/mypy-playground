FROM python:3.14.0a3-slim

WORKDIR /tmp
COPY ./requirements.txt /tmp/

RUN pip install -r requirements.txt \
        && rm -rf /tmp/requirements.txt \
        && rm -rf /root/.cache

USER nobody
CMD ["mypy"]
