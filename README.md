# Supported tags and respective `Dockerfile` links

-	[`latest` (*Dockerfile*)](https://github.com/tool-dockers/docker-mkpasswd/blob/master/Dockerfile)

# Quick reference

-	**Where to get help**:
	[the tool-dockers online doc](http://doc.tool-dockers.com/), [the tool-dockers Support Organization](https://support.tool-dockers.com/)

-	**Where to file issues**:
	[https://github.com/tool-dockers/docker-mkpasswd/issues](https://github.com/tool-dockers/docker-mkpasswd/issues)

-	**Maintained by**:
	[the tool-dockers Team](https://github.com/tool-dockers/docker-mkpasswd)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))
	[`amd64`](https://hub.docker.com/r/amd64/whois/)

-	**Source of this description**:
	[docs repo's `tool-dockers/` directory](https://github.com/tool-dockers/docker-mkpasswd/tree/master) ([history](https://github.com/tool-dockers/docker-mkpasswd/commits/master))

-	**Supported Docker versions**:
	[the latest release](https://github.com/docker/docker-ce/releases/latest) (down to 1.6 on a best-effort basis)

# What is mkpasswd?

The package contains **mkpasswd**, a features-rich front end to the password encryption function crypt(3).

**mkpasswd** generates passwords and can apply them automatically to users. This tool is useful for Ansible playbooks in scenarios where you want to put a password (for a database) into the playbook but don't want it in the clear.

# How to use this image

## mkpasswd

Command line help is provided:

```bash
docker run --name whois --rm tooldockers/mkpasswd:latest -h
```

To generate a SHA-512 encrypted password:

```bash
docker run --name whois --rm tooldockers/mkpasswd:latest -m SHA-512 [PASSWORD [SALT]]
```
