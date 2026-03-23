FROM python:3.11-slim

WORKDIR /app

RUN pip install --no-cache-dir wsgidav cheroot

RUN mkdir -p /obsidian_vault

COPY wsgidav.yaml /app/wsgidav.yaml

EXPOSE 37501

CMD ["wsgidav", "--config", "/app/wsgidav.yaml"]