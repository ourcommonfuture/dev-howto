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

### [Sublime Text](http://www.sublimetext.com/3)

An amazing text editor with extensive capabilities, especially thanks to the [package manager](https://sublime.wbond.net/installation). 

**N.B.:** The project capabilities of Sublime is amazingly useful.

1. If you already have some files open from the same project, go to `Project>Save project as...` and save the file outside your github folder (it is personnal and therefore shouldn't be on a github repo). Then, you can go to `Project>Add folder to project...` and select your project folder. It will appear on the left and allows you to access rapidly all your project files!
2. You can create/open another project. When you have multiple project, you can switch from one another with the shortcut `Cmd+ctl+p`. Sublime will remember all the files you had open.
3. The configuration through the whole project is useful as well, see the [documentation](https://www.sublimetext.com/docs/3/projects.html). A good practice is to set the tab settings, here is an example:

```json
{
  "folders":
  [
    {
      "path": "path/to/your/project"
    }
  ],
  "settings":
  {
    "tab_size": 4,
    "translate_tabs_to_spaces": false
  }
}
```

### [iTerm](http://iterm2.com/)

A waty better terminal for your mac.

### [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

Great shell improver. Usually already on your vagrant box. ;)
