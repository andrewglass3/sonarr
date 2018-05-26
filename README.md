# sonarr
Sonarr in docker

This is a simple docker-compose for running Sonarr in docker. Using linuxserver/sonarr image from dockerhub:

    environment:
      - TZ=Europe/London
      - PUID=1000
      - PGID=1000
    volumes:
      - /mnt/docker/sonarr:/config
      - /mnt/plex/tv:/tv

All of my docker containers run under PUID and PGID 1000 - to see your id that you run docker commands as use the command 'id'
Volumes are ordered localhost strage:inside container location. 

I hope this is helpful to you and big thanks to linuxserver.io for the sonarr image.
