# Libreflip Deployment

A collection of build pipeline tools and `Dockerfile`s to build libreflip platform targets. Is displayed as a single repo on dockerhub which means you need to provide the correct tags to pull images.

 - `base-armhf` is the base image for armhf targets
 - `base-arm64` is the base image for 64bit arm targets
 - `base-x86_64` is the base image for "normal" 64bit x86 targets

The libreflip specific targets include

- `sans-ci` is used internally for the travis CI runners. Produces the other images.
- `sans-server` includes a run environment and instructions to get the Libreflip server stack running. Available only on `armv7`
- `sans-worker` is a conveniently deployable image to install work runners on other platforms. Available for `armv7`, `arm64` and `x86_64`


## Contribute

Pull Requests are welcome, please look at the coding style before making additions. Maybe open an issue before a PR first too.