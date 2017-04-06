# ansible-docker-osx
Use ansible to ease ths installation of Docker Toolbox. 
Docker-machine-nfs increase the read/write access to your filesystem between OSX and your VM.

Install the requirements 
```bash
brew install python
pip install ansible
```

Clone the project
```bash
git clone https://github.com/anthonykgross/ansible-docker-osx.git
cd ansible-docker-osx
sudo ansible-galaxy install -r requirements.yml
```

If you want to install Docker Toolbox + docker-machine-nfs
```bash
ansible-playbook install.yml 
```

If you want to uninstall Docker Toolbox + docker-machine-nfs
```bash
ansible-playbook uninstall.yml 
```

**Note** : You could have an issue during the installation if you've tried to install Docker Toolbox before. Run the ```uninstall``` part to fix it and run ```install``` again.

## Creator
**Anthony K GROSS**
- <http://anthonykgross.fr>
- <https://twitter.com/anthonykgross>
- <https://github.com/anthonykgross>

## Copyright and license
Code and documentation copyright 2017. Code released under [the MIT license](https://github.com/anthonykgross/ansible-docker-osx/blob/master/LICENSE).