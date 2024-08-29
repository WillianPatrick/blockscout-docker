FROM blockscout/blockscout:latest

COPY ./config/.. /config
#VOLUME [ "./logs/:/app/logs/", "./config:/config" ] 

EXPOSE 4000:4000
CMD sh -c "bin/blockscout eval \"Elixir.Explorer.ReleaseTasks.create_and_migrate()\" && bin/blockscout start"
