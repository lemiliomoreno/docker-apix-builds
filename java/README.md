# Docker Java build

```bash
# build docker image
docker build -t sample-java:1.0.0 . --progress plain --no-cache

# run docker image
docker run -p 80:8080 sample-java:1.0.0
```
