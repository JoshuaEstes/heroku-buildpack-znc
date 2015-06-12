znc buildpack for Heroku
========================

This buildpack is used to install [ZNC] on Heroku.

## Usage

Add this build pack to your Heroku app.

> NOTE: You can create a new app or use an existing one

```shell
heroku buildpacks:add https://github.com/JoshuaEstes/heroku-buildpack-znc
```

## Configuration

Your app should match this layout:

```shell
.
├── Procfile
├── configs/
│   └── znc.conf
├── moddata/
├── modules/
├── users/
└── znc.pem
```

See [ZNC Documentation] on what goes in all those directories and files

## Sample `Procfile`

```
znc: bin/znc
```

## Sample `configs/znc.conf`

```
```

> NOTE: Make sure you use `$PORT` so it adheres to Heroku's policies.

## Change Log

See [CHANGELOG.md]

## License

See [LICENSE]

[ZNC]: http://znc.in
[ZNC Documentation]: http://wiki.znc.in/ZNC
[CHANGELOG.md]: https://github.com/JoshuaEstes/heroku-buildpack-znc/blob/master/CHANGELOG.md
[LICENSE]: https://github.com/JoshuaEstes/heroku-buildpack-znc/blob/master/LICENSE
