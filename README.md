# Wallarm FAST custom detects

## HOWTO use

Connect with Wallarm FAST by local directory mapping
```
$ docker run -p 8888:8080 -v /path/to/your-own-detects-in-yaml:/opt/custom_extensions -e WALLARM_API_TOKEN=xxx wallarm/fast
```
by GIT repository mapping:
```
$ docker run -p 8888:8080 -e GIT_EXTENSIONS=https://github.com/wallarm/fast-detects -e WALLARM_API_TOKEN=xxx wallarm/fast
```
