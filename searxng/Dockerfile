FROM docker.io/searxng/searxng:latest

# Passa a root per copiare i file
USER root

# Copia i file di configurazione
COPY limiter.toml /etc/searxng/limiter.toml
COPY settings.yml /etc/searxng/settings.yml

# Cambia i permessi per l'utente searxng
RUN chown -R searxng:searxng /etc/searxng

# Torna all'utente originale
USER searxng