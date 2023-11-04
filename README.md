# family_hub
This is a platform in which you can interact as  a family such as playing games or planning your TODOs 


1. Installation zsh on your raspberrypi
https://divinenanny.nl/blog/2021-08-07-install-oh-my-zsh-on-raspberry-pi/

2. create pyenv for using multiple python versions

Follow the instruction of the website. However in the second step is telling you to edit your `~/.bashrc`. When using zsh as shell, edit `~/.zshrc`.

In step five you go to the repo's path and execute the following comand, after updating the pyenv :

```shell
pyenv install 3.12.0

pyenv local 3.12.0
```
 
https://www.samwestby.com/tutorials/rpi-pyenv.html

3. creating the virtual environment

Create a new virtual environment:

```shell
$ pyenv virtualenv 3.12.0 venv_family_hub
```

https://github.com/pyenv/pyenv-virtualenv#using-pyenv-virtualenv-with-pyenv:~:text=%24%20pyenv%20virtualenv%202.7.10%20my%2Dvirtual%2Denv%2D2.7.10

ATTENTION:

Solving problem activating the virtual env check if you the shell configuration looks like following:

```shell
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```


https://github.com/pyenv/pyenv-virtualenv/issues/387#issuecomment-850839749
