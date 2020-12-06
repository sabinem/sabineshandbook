*******
Docker
*******

Volumes
========

Sometimes mounts can go sour because a file was misspelled and docker created a directory instead of the file:

```
Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type
```

- delete the directory
- `docker ps -a`
- `docker container rm -v`
- now get docker up again