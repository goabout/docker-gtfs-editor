Conveyal GTFS Editor Docker image
=================================

This project contains a Docker image for the Conveyal
[GTFS Editor](https://github.com/conveyal/gtfs-editor). It is available from
Docker Hub in the
[`goabout/gtfs-editor` repository](https://hub.docker.com/r/goabout/gtfs-editor/).

## Usage

    docker run \
        -v /path/to/application.conf:/opt/gtfs-editor/conf/application.conf:ro \
        -v /path/to/data:/opt/gtfs-editor/data \
        -p 80:9000 \
        goabout/gtfs-editor

The application will be installed at `/opt/gtfs-editor'. The default data
location, `/opt/gtfs-editor/data` is a volume. Port 9000 is exposed.
