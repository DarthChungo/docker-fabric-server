# Docker Minecraft Server

A simple docker image to run a minecraft server in a docker container.
Automatically downloads the minecraft server jar from the desired link and runs it.
You can mount `/mc/server` as a volume to your host machine to persist data across container launches.


## Building and running

```bash
git clone git@github.com:DarthChungo/docker-minecraft-server.git
cd docker-minecraft-server
```

```bash
docker build -t docker-minecraft-server .
```

```bash
docker run -d -p 25565:25565 -v $(pwd)/data:/mc/server docker-minecraft-server
```


# License

Docker Minecraft Server, a simple docker image to run a minecraft fabric server 

Copyright © 2023 Antonio de Haro

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
