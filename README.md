# try-without-install

Curated list of commands that can be installed with Docker as package manager without the need to mutate your system with snap/apt/rpm/whatever.

It's easy, want to install `aws` CLI?

```shell
curl https://raw.githubusercontent.com/lucabrunox/try-without-install/refs/heads/main/bin/aws > /usr/local/bin/aws
chmod +x /usr/local/bin/aws
```

If that's too long you can install the `twi` wrapper:

```shell
curl https://raw.githubusercontent.com/lucabrunox/try-without-install/refs/heads/main/bin/twi > /usr/local/bin/twi
chmod +x /usr/local/bin/twi
```

And now to install `aws` you can do:

```shell
twi aws
```

If you want to see which packages have been installed this way on your system:

```shell
grep try-without-install /usr/local/bin/*
```