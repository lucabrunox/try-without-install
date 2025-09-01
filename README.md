# try-without-install

A curated list of commands that can be installed with Docker as package manager without the need to mutate your system with snap/apt/yum/etc.

For example to install the `aws` CLI you can:

```shell
sudo curl -f https://raw.githubusercontent.com/lucabrunox/try-without-install/refs/heads/main/bin/aws -o /usr/local/bin/aws && sudo chmod +x /usr/local/bin/aws
```

Then you can use `aws` like a normal command.

-----

Or you can also use the `twi` wrapper:

```shell
sudo curl -f https://raw.githubusercontent.com/lucabrunox/try-without-install/refs/heads/main/bin/twi -o /usr/local/bin/twi && sudo chmod +x /usr/local/bin/twi
```

Then to install `aws`:

```shell
sudo twi aws
```

-----

If you want to see which commands have been installed this way on your system:

```shell
grep -R try-without-install /usr/local/bin
```
