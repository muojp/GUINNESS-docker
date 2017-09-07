# GUINNESS-docker: A Docker image making GUINNESS even easier to evaluate

## GUINNESS?

=> <https://github.com/HirokiNakahara/GUINNESS>

## GUINNESS-docker?

![GUINNESS-docker](https://raw.githubusercontent.com/muojp/GUINNESS-docker/master/guiness-docker.png)

 - A Docker image leverages NVIDIA's official CUDA image: <https://hub.docker.com/r/nvidia/cuda/>
 - You can easily start evaluating GUINNESS via Web Browsers
 - Fully functional (boosted by GPUs) when combined with nvidia-docker: <https://github.com/NVIDIA/nvidia-docker>
 - NOTE: GUI itself and CPU-only training should work under Windows 10 and macOS, but nvidia-docker doesn't currently support those environments to proxy native GPU into Docker containers.

## Usage

1. Start Docker container

```
$ docker run -it --rm -v/path/to/datadir:/data -p6080:6080 muojp/GUINNESS:latest
```

2. Access GUI using Web Browsers: Open <http://localhost:6080/>

3. Enjoy!

4. Type Ctrl-C into Docker console to terminate the container.

## Tutorials and how-tos

Please read through the original README: <https://github.com/HirokiNakahara/GUINNESS/blob/master/README.md>

## Legal notice

Composer of this image have nothing to do with GUINNESS' original authors.
Please don't ask questions about GUINNESS-docker to original authors. Instead, please file an issue on this repository.

## LICENSE

MIT
