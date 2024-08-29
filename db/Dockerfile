FROM postgres:15

# Qual a necessidade real???
#USER root
#RUN chown -R 2000:2000 /var/lib/postgresql/data
#VOLUME ["./data:/var/lib/postgresql/data"]
#USER 2000:2000

EXPOSE 7432:5432

CMD ["postgres", "-c", "max_connections=200", "-c", "client_connection_check_interval=60000"]

HEALTHCHECK --interval=10s --timeout=5s --start-period=10s --retries=5 CMD pg_isready -U blockscout -d blockscout
