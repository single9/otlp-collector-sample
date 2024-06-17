# OTLP Collector

## General

```
docker run -p 4317:4317 -p 4318:4318 --rm -v $(pwd)/collector-config.yaml:/etc/otelcol/config.yaml otel/opentelemetry-collector
```

## AWS

```
docker run -p 4317:4317 -p 4318:4318 --rm -v $(pwd)/collector-config.yaml:/etc/otelcol/config.yaml --env-file `pwd`/.env public.ecr.aws/aws-observability/aws-otel-collector
```
