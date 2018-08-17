
## RUN Interactively

```
docker run --rm -it \
    -v `pwd`:/data \
    charlestg/ffmpeg_centos7 ffmpeg
```

## Run As Alias

```
### Create Alias
alias ffmpeg='docker run --rm -it --name ffmpeg -v `pwd`:/data charlestg/ffmpeg_centos7 ffmpeg'
alias ffprobe='docker run --rm -it --name ffprobe -v `pwd`:/data charlestg/ffmpeg_centos7 ffprobe'

### Run with Alias
ffmpeg --help
```