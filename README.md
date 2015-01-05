# fig-drupal_stack

A fig configuration that sets up an Apache-PHP-MySQL stack with some additional Drupal containers.

Note this is just a proof-of-concept. You very likely don't want to use this in a production environment.

# Install

Before you start, you need to know whether you have to run Docker commands using `sudo` or not. If so, prefix all `fig` and `docker` commands with `sudo` below.

1. [Install docker](https://docs.docker.com/installation/).
    * Test it works with `docker run hello-world`
2. [Install fig](http://www.fig.sh/install.html).
    * Test it works with `fig --version`
3. Put a PHP web application inside the webroot folder (e.g.: [Drupal](https://drupal.org/project/drupal)).
    * If the web application requires write-access to a certain file or folder, you'll have to set permissions with `chmod g+w $path ; chown -R :33 $path`.
    * If the web application has trouble writing to the database, you'll have to set permissions with `chown -R :999 db`.

# Usage

1. From a terminal, run:

        fig up

You can now run the PHP web application by visiting http://localhost/
