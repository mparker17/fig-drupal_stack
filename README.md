# fig-amp_stack

A fig configuration that sets up an Apache-PHP-MySQL stack using Docker.

Note this is just a proof-of-concept. You very likely don't want to use this in a production environment.

# Install

Before you start, you need to know whether you have to run Docker commands using `sudo` or not. If so, prefix all `fig` and `docker` commands with `sudo` below.

1. [Install docker](https://docs.docker.com/installation/).
    * Test it works with `docker run hello-world`
2. [Install fig](http://www.fig.sh/install.html).
    * Test it works with `fig --version`

# Usage

1. From a terminal, run:

        fig up
