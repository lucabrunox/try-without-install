# try-without-install

Curated list of commands that can be installed with Docker as package manager without the need to mutate your system with snap/apt/rpm/whatever.

Install the `twi` wrapper:

```shell
sudo curl -f https://raw.githubusercontent.com/lucabrunox/try-without-install/refs/heads/main/twi -o /usr/local/bin/twi && sudo chmod +x /usr/local/bin/twi
```

And now to install `aws` you can do:

```shell
twi aws
```

If you want to see which commands have been installed this way on your system:

```shell
grep try-without-install /usr/local/bin/*
```