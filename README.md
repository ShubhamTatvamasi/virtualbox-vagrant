# virtualbox-vagrant

install virtualbox:
```bash
sudo apt install virtualbox
```

install vagrant:
```bash
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install vagrant
```

install plugins:
```bash
vagrant plugin install vagrant-vbguest
```

