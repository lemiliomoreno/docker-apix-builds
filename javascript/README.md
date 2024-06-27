# Docker Javascript build

```bash
# build docker image
docker build -t sample-frontend:1.0.0 . --progress plain --no-cache

# run docker image
docker run -p 80:80 sample-frontend:1.0.0
```
