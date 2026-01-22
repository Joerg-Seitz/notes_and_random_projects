# Helpful scripts/notes/commands

## Failing downloads/updates

Can happen when CDN or mirrors arent correctly referenced.
Can be fixed by running `sudo pacman -S cachyos-mirrorlist` and afterwards rating the mirrors with `sudo cachyos-rate-mirrors`

In `/etc/pacman.d` the following lines were commented out (and uncommented back in) in order to force CachyOS to use functional mirrors.
``` 
Server = https://aur.cachyos.org/repo/$arch_v3/$repo
Server = https://cdn.cachyos.org/repo/$arch_v3/$repo
```


Afterwards running `sudo payman -Syu` successfully updated

## Becoming superuser/sudo for the current shell

Sudo session without keeping current ENV

```
sudo -i
``` 

Sudo session with keeping current ENV

```
sudo -s
```

