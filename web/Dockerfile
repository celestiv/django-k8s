FROM python:3.9.10-slim

WORKDIR /app

COPY . /app

RUN python -m venv /opt/venv


RUN /opt/venv/bin/pip install --upgrade pip && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x entrypoint.sh


CMD ["/app/entrypoint.sh"]