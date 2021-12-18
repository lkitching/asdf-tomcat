#asdf-tomcat
[Apache Tomcat](https://tomcat.apache.org/) plugin for [asdf](https://asdf-vm.com/).

## Install

Ensure [asdf](https://asdf-vm.com/) is installed and then install the plugin with

```bash
asdf plugin add tomcat https://github.com/lkitching/asdf-tomcat
```

## Usage
Once installed, the plugin can be used via asdf to list and install available versions e.g.

```bash
asdf list all tomcat
asdf install tomcat 9.0.56
```

The plugin exports the binaries within the `/bin` directory of the distribution. If the asdf shims directory is on your `PATH`
these should be available:

```
# start tomcat server
catalina.sh
```

The plugin sets `CATALINA_HOME` to the location of the current version specified in `.tool-versions`.