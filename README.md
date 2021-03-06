# Ubuntu baseimage Meteor Docker Build
Ubuntu baseimage for build and run Meteor applications inside docker container.

Fetures:

- Small Ubuntu image based on [`phusion/baseimage-docker`](https://github.com/phusion/baseimage-docker) (look why and read about image features)
- Meteor is allready preinstaled in this image.
- Your aplication will be builded inside docker container.
- No Meteor or Nodejs instalation needed on build host.
- Nodejs is linked from Meteor installation for maximum comapatibylity.
- You can add volume linked to `/var/log/meteor.log` for Meteor logging.
- You can add more serivces or deamons to run inside container for example [`memcached`](https://github.com/phusion/baseimage-docker#adding-additional-daemons)

## Project state
> Currently in beta testing! [@TODO](#todo)

## Versions
> [@TODO](#todo)

## How to use

See `example` folder how to build your application docker container. Simply copy files from example folder into your Meteor project. Setup options in `docker-build.sh` file and run `sh docker-build.sh`.

## TODO

- [ ] Add image versions depended on baseimage and Meteor versions
- [ ] Run NodeJS App under Meteor user
- [ ] Meteor proper loging with date-time and maybe to syslog-ng
- [ ] Production ready realease
- [ ] Add example scripts for install Imagemagick, Graphicmagick, etc.

## Credits

- Builded from [`phusion/baseimage-docker`](https://github.com/phusion/baseimage-docker) image
- Inspired by [`tozd/docker-meteor`](https://github.com/tozd/docker-meteor) repository.
- Authors:
	- [Martin Bucko](https://github.com/MartinBucko)

***Thanks guys!***

## License

[MIT](https://github.com/Treecom/baseimage-meteor/blob/master/LICENSE)
