# Docksible

Docksible is a script that helps you manage easily docker containers and test deployments with Ansible.

- [Docksible](#docksible)
  - [Automating with Docksible](#automating-with-docksible)
    - [Make docksible executable](#make-docksible-executable)
    - [Docksible commands and options](#docksible-commands-and-options)
  - [Examples](#examples)
  - [Thanks to](#thanks-to)

---

**Docksible** is a script that allows to you create **docker containers on the fly by specifying container name(s)**. These containers are based on a debian docker image. Take a look at here if you want more details from the image used [debian-systemd-ssh](https://github.com/sram-z/debian-systemd-ssh).

In the background **Docksible** will create for you a user account (the same as the current user) with sudo privileges. The given name will also be the hostname of the container.

---

## Automating with Docksible

### Make docksible executable

At first, make sure that the `docksible` script is executable.

`chmod +x docksible`

### Docksible commands and options

```console
docksible <command> [option]

Commands:
  create:   create one or more containers separeted by a comma.
 
 ansible:   create minimal structure for ansible.
 
   purge:   delete all container(s) created by docksible.

Options:      
    - k :   permit to initialise containers with your ssh key
            dockesible create -k <your_ssh_public_key>
            It supposed that your ssh key is stored in the default directory: 
            ~/.ssh/key_ssh.pub

    - h :   help
```

## Examples

Coming soon...

## Thanks to

- [priximmo](https://gitlab.com/xavki/presentations-scripting/-/blob/master/shell/deploy.sh) for script inspiration.
  