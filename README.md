# Minimal Godot Engine Docker image

This image is based on a minimal Alpine Linux image that includes glibc. It provides the official Linux server 64-bit 3.0.1-stable build of Godot Engine along with the official templates.

The primary application is for automating Godot Engine builds.

Godot Engine is located at ```/bin/godot``` and the templates are installed in ```/root/.godot/templates```.

### Usage example (Gitlab CI)

The source repository contains a ```Vagrantfile``` who provides Docker and Gitlab Runner. It can be used to test your Gitlab CI configuration (see ```.gitlab-ci.yml``` in the source repository):

    $ gitlab-runner exec docker <job name>
   
There is no need to register the runner first.

### Credits

Rafał Zawadzki: https://hub.docker.com/r/bluszcz/godot/
