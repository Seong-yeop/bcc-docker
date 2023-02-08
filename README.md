From your host shell:
```bash
sudo docker run -it  \
-v /lib/modules:/lib/modules:ro  \
-v /usr/src:/usr/src:ro \
-v /etc/localtime:/etc/localtime:ro \
--privileged --pid=host --workdir /usr/share/bcc/ szp2030/bcc:v1.0
```

Now, from the container shell, you can try the various pre-installed bcc tools.

For examples, please refer to the [bcc tutorial](https://github.com/iovisor/bcc/tree/master/docs/tutorial.md#1-general-performance).
