# Docker .NET build

```bash
# build docker image
docker build -t sample-dotnet:1.0.0 . --progress plain --no-cache

# run docker image
docker run -p 80:80 sample-dotnet:1.0.0
```
