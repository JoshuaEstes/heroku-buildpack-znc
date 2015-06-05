znc buildpack for Heroku
========================

This buildpack is used to install [znc] on Heroku.

## Usage

Add this build pack to your Heroku app.

>> You can create a new app or use an existing one

```shell
heroku buildpacks:add https://github.com/JoshuaEstes/heroku-buildpack-znc
```

## Configuration

Your app should match this layout

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

See znc documentation on what goes in all those directories and files

## Change Log

## License

MIT


[znc]: http://znc.in
