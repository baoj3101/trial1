# AP CSP Linux Notebook

## Setup github

### ssh-kengen

* ssh-keygen — authentication key generation, management and conversion

> pi@rpi:~ $ ssh-keygen
> Generating public/private rsa key pair.
> Enter file in which to save the key (/home/pi/.ssh/id_rsa): 
> /home/pi/.ssh/id_rsa already exists.
> Overwrite (y/n)? y
> Enter passphrase (empty for no passphrase): 
> Enter same passphrase again: 
> Your identification has been saved in /home/pi/.ssh/id_rsa.
> Your public key has been saved in /home/pi/.ssh/id_rsa.pub.
> The key fingerprint is:
> SHA256:dqKaKWSht5d55iI7NXi/S/XryRSoITzRkOoL8H5sOBI pi@rpi
> The key's randomart image is:
> +---[RSA 2048]----+
> |    ..           |
> |    .o           |
> |   .. .          |
> |. o. .   .       |
> |.+ o+ . S o      |
> |E B +o * + .     |
> | B B =+   o      |
> |. X O=+  o o     |
> | ..X+=+o .=      |
> +----[SHA256]-----+

* Copy the whole text of the public ssh key and then log into github.

> pi@rpi:~ $ cat ~/.ssh/id_rsa.pub

* In github, under "Settings" => "SSH and GPG keys" => "New SSH key"
** Enter a title such as "school Pi"
** Paste ssh public key into the textbox
** Click "Add ssh key"
** Enter github password to save

* In linux terminal, use "ssh git@github.com" to validate the connection.
> pi@rpi:~ $ ssh git@github.com
> PTY allocation request failed on channel 0
> Hi baoj3101! You've successfully authenticated, but GitHub does not provide shell access.
> Connection to github.com closed.







