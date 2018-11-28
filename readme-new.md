# Influxdb Beat Export

## Install

### Build

```
docker build . -t dashbase/beat-exporter:nightly
```

## Usage

Plz modify your env and run:

```
docker run -e INFLUXDB_URL=http://localhost:8086 -e INFLUXDB_USERNAME=username -e INFLUXDB_PASSWORD=password -e INFLUXDB_DB=dashbase_filebeat dashbase/beat-exporter:nightly "-beat.uri http://localhost:5066"
```

