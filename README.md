# provision-osx
Provisioning details for OSX

## Before running

#### GitHub
Generate a new SSH-key for use with GitHub.

```shell
ssh-keygen -t rsa -b 4096 -C "your.github.email@domain.com"
sudo chmod 600 ~/.ssh/id_rsa
sudo chmod 600 ~/.ssh/id_rsa.pub
sudo chmod 755 ~/.ssh/
ssh-add -K /path/to/generated/private_key
pbcopy < /path/to/generate/key
```

Go to [GitHub](https://github.com/settings/ssh) and paste your newly generated key. Test your GitHub access by running

```shell
ssh -T git@github.com
```

```shell
git clone git@github.com:k-olthof/provision-mac.git
cd provision-mac
./provision.sh
```
