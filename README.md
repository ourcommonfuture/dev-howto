dev-howto
=========

Here is a little guide on how to get some correct dev tools and environement along with some interesting ressources.

Please add your own as well!

## The basic: Vagrant

In order to all have the same dev. environement to develop our application, we use Vagrant, a command-line virtualization tool. Here is a quick step by step:

1. [Download](https://www.virtualbox.org/wiki/Downloads) and install VirtualBox.
2. [Download](https://www.vagrantup.com/downloads.html) and install Vagrant.
3. Clone one of our repo. It will contains a `Vangrantfile` on the root, which contains all the virtualization configuration. Once your are `cd` in your repository forlder, just run those commands:

```bash
# First, initiate and run your virtualisation box
vagrant up
# (please note that you will need to "up" your box every time you run your computer or after a certain timeout)
# Then, you can ssh into it
vagrant ssh
```

You will then be able to run commands into the right environement.

**Important**: your github folder containing the `Vagrantfile`, will be accessible into your virtual box into the `/vagrant/` forlder.

## Tools

Those tools are more recommended than really required.

- [Sublime Text](http://www.sublimetext.com/3): An amazing text editor with extensive capabilities, especially thanks to the [package manager](https://sublime.wbond.net/installation). 
- [iTerm](http://iterm2.com/): A waty better terminal for your mac.
- [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh): Great shell improver.
