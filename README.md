# docker-aosp

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

![Docker Version](https://img.shields.io/docker/v/appknox/aosp/latest)
![CI](https://github.com/appknox/docker-aosp/actions/workflows/docker-image.yml/badge.svg?branch=master)
![Pulls](https://img.shields.io/docker/pulls/appknox/aosp.svg)


Docker images for Android modules or apps that really need to be built inside the [AOSP](https://source.android.com/) source tree. This allows you to access all private APIs in both Java and C++ land. Doing that is usually a massive pain, and definitely not recommended for any application. Even with these helper images, it's not exactly a walk in the park. Furthermore, by using private APIs you risk your module or app crashing on random devices.
## Features

* Create local AOSP mirrors
* Checkout AOSP branches or tags (from your local mirror or directly)
* Build your own modules inside any checked out AOSP branches
* Supports JDK8 (with appknox/aosp:latest)

Available as [appknox/aosp](https://hub.docker.com/r/appknox/aosp) in the Docker Hub Registry.

## Requirements

* [docker](https://www.docker.com/)
* Vast amounts of disk space. A local mirror currently takes roughly 60GB, and each checked out branch roughly 20-30GB after building your module and its deps.
* Knowledge of AOSP.
## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

See [LICENSE](LICENSE).
Borrowed from OpenSTF Project. Not a Fork, since the project is archived.
Copyright © The OpenSTF Project. All Rights Reserved.
Copyright © XYSEC Labs Pvt Ltd. All Rights Reserved.
