# My Insurgency: Sandstorm configs

## Things you need to do to use them

### Authentication

First, you need to go get yourself a [mod.io account](https://mod.io/g), then get your [OAuth Access token](https://mod.io/me/access).

Once you have those, create `ismc2/config/ini/GameUserSettings.ini` with the following content:

```ini
[/Script/ModKit.ModIOClient]
bHasUserAcceptedTerms=True
AccessToken=<Your Access Token Here>
```

### Get Docker/Podman

[Docker](https://docker.com) is a service that allows for containerization of software. It requires an account now :(

[Podman](https://podman.io/) is an open source (and I think nicer) alternative to Docker. It also doesn't run as a daemon and doesn't require an account. Thank you RedHat!

### Edit the configs

Not gonna explain all that here, but you can [read the documentation on mod.io](https://mod.io/g/insurgencysandstorm/r/server-admin-guide).

Some things are automated already in the docker image. Setting up the `.env` file and some other configuration is [documented here](https://github.com/AndrewMarchukov/insurgency-sandstorm-server-dockerize)

### Let 'er rip!

```sh
docker compose up
```

## Credits

Big thank you to @AndrewMarchukov and the folks at [mod.io](https://mod.io) for providing the docker image and tutorial, respectively.
