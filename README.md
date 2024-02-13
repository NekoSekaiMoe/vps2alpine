# VPS2ALPINE

> Install Alpinelinux on your VPS, no matter what the current OS is.

## Usage

1. Install curl with your current package manager

2. Run this script

```
$ curl -OL https://raw.githubusercontent.com/SekaiMoe/vps2alpine/main/vps2alpine
$ chmod +x vps2alpine
$ sudo ./vps2alpine #[OPTIONS]
```

3. Sync data and reboot

```
$ sudo $SHELL -c 'sync && reboot -f'
```

4. Connect to server after about 3 minutes.

```
# the root password from the original system (or by using vps2alpine as password if no root password was set).
$ ssh root@your-server-ip
```

5. Change your root password

```
passwd
```

### Options

```
-h Show help messages.
-s Set OS version, For example "-s Leap-15.3" (Default: Tumbleweed).
-a Set default zone (Default: 'Asia/ShangHai').
-m Set mirror address (Default: http://dl-cdn.alpinelinux.org/alpine).
```

## Credits

This project is based on [vps2arch](https://github.com/drizzt/vps2arch)

## License

GNU General Public License 3.0
