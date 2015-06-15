# LatestMe  

LatestMe automatically updates running containers with their latest image version in case a security vulnerability is found.

The approach taken by LatestMe is to replace running container with a new image. This is instead of standard methods to apply security patches, "apt-get" and "yum update" mechanisms, which break the concept of immutable containers.

## How does it work

1. Identify that a running container has security vulnerability.
2. Search Docker registry for updated image.
3. Verify that security vulnerability is fixed in the updated image.
4. Replace running container with updated image.
