# Quick reference

-	**Maintained by**:
	[tool-dockers](https://github.com/tool-dockers/docker-mkpasswd)

-	**Where to get help**:
	[the tool-dockers Community Slack][slack]

# Supported tags and respective `Dockerfile` links

-	[`latest` (*Dockerfile*)](https://github.com/tool-dockers/docker-mkpasswd/blob/master/Dockerfile)

# Quick reference (cont.)

-	**Where to file issues**:
	[https://github.com/tool-dockers/docker-mkpasswd/issues](https://github.com/tool-dockers/docker-mkpasswd/issues)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))
	[`amd64`](https://hub.docker.com/r/amd64/mkpasswd/)

-	**Source of this description**:
	[docs repo's `tool-dockers/` directory](https://github.com/tool-dockers/docker-mkpasswd/tree/master) ([history](https://github.com/tool-dockers/docker-mkpasswd/commits/master))

-	**Supported Docker versions**:
	[the latest release](https://github.com/docker/docker-ce/releases/latest) (down to 1.6 on a best-effort basis)

# What is mkpasswd?

[![tool-dockers][logo]][website]

The package contains **mkpasswd**, a features-rich front end to the password encryption function crypt(3).

**mkpasswd** generates passwords and can apply them automatically to users. This tool is useful for Ansible playbooks in scenarios where you want to put a password (for a database) into the playbook but don't want it in the clear.

# How to use this image

## mkpasswd

Command line help is provided:

```bash
docker run --name mkpasswd --rm tooldockers/mkpasswd:latest -h
```

To generate a SHA-512 encrypted password:

```bash
docker run --name mkpasswd --rm tooldockers/mkpasswd:latest -m SHA-512 [PASSWORD [SALT]]
```

# License

View [license information](https://raw.githubusercontent.com/tool-dockers/docker-mkpasswd/master/LICENSE) for the software contained in this image.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.

## License

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

## About

[tool-dockers][website] maintains and funds this project.

  [logo]: https://avatars3.githubusercontent.com/u/57697117?s=60&v=4
  [website]: https://continuul.solutions
  [slack]: https://continuul.slack.com
