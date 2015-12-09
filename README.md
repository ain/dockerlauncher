# dockerlauncher

Docker Compose services starter for Debian init system.

## Requirements

- Debian OS
- Source code of project(s) installed in separate `/var/www/<website>` folders
- Every project includes Docker Compose file, e.g. `/var/www/<website>/docker-compose.yml`

## Installation

```
curl -L https://github.com/ain/dockerlauncher/raw/master/dockerlauncher > /etc/init.d/dockerlauncher
```

```
chmod +x /etc/init.d/dockerlauncher
```

To launch services on every boot:

```
update-rc.d dockerlauncher defaults
```

## Licence

Copyright © 2015 Ain Tohvri. Licenced under [GPL-3](LICENSE).
