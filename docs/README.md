# Headline

> An awesome project.

## sec 1

text

## sec 2

- even
- more
- text

When working with Node.js, you might encounter situations where you need to install multiple versions of the runtime.

For example, maybe you have the latest version of Node set up on your machine, yet the project you’re about to start working on requires an older version. Or maybe you’re upgrading an old Node project to a more modern version and it would be handy to be able to switch between the two while you make the transition.

Without a good tool, this would mean spending a lot of time and effort manually uninstalling and reinstalling Node versions and their global packages. Fortunately, there’s a better way!
Introducing nvm

nvm stands for Node Version Manager. As the name suggests, it helps you manage and switch between different Node versions with ease. It provides a command-line interface where you can install different versions with a single command, set a default, switch between them and much more.
OS Support

nvm supports both Linux and macOS, but that’s not to say that Windows users have to miss out. There’s a second project named nvm-windows that offers Windows users the option of easily managing Node environments. Despite the name, nvm-windows is not a clone of nvm, nor is it affiliated with it. However, the basic commands listed below (for installing, listing and switching between versions) should work for both nvm and nvm-windows.

## Installation

Let’s first cover installation for Windows, macOS and Linux.
Windows

First, we need to do a little preparation:

    uninstall any existing versions of Node.js
    delete any existing Node.js installation directories (such as C:\Program Files\nodejs)
    delete the existing npm install location (such as C:\Users\<user>\AppData\Roaming\npm)

After this, download and run the latest stable installer and you should be good to go!
macOS/Linux

Unlike Windows, removing previous Node and npm installations in macOS and Linux is optional. If this is something you want to do, there are plenty of good resources available online. For example, here’s how to remove Node on macOS and on Linux. And here’s how you can remove any previous npm installation you might have.

You can install nvm using cURL or Wget. On your terminal, run the following:

### With cURL:

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.35.2/install.sh | bash
```

### Or with Wget:

```
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.35.2/install.sh | bash
```
