# Docker as package manager

A curated list of commands that can be installed with Docker as package manager without the need to use snap/apt/yum/etc.

For example to install the `aws` CLI you can:

```shell
sudo curl -f https://raw.githubusercontent.com/lucabrunox/docker-package-manager/refs/heads/main/bin/aws -o /usr/local/bin/aws && sudo chmod +x /usr/local/bin/aws
```

Then you can use `aws` like a normal command.

-----

Or you can also use the `dpm` wrapper:

```shell
sudo curl -f https://raw.githubusercontent.com/lucabrunox/docker-package-manager/refs/heads/main/bin/dpm -o /usr/local/bin/dpm && sudo chmod +x /usr/local/bin/dpm
```

Then to install `aws`:

```shell
sudo dpm aws
```

-----

If you want to see which commands have been installed this way on your system:

```shell
grep -R docker-package-manager /usr/local/bin
```
