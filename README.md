ShellShocker
============

<img src="https://github.com/ArchimedesPi/shellshocker/raw/master/shellshocker_server/assets/images/shellshock-logo.png" alt="ShellShocker" align="right" />

If you don't know what the ShellShock Bash exploit is, you should probably Google it.
Now that you know...

### What is this for?
ShellShocker tests a website for vulnerability to the ShellShock bug.
There's a command-line tool for doing testing, and a deployable Flask-powered
ShellShock testing website (punch in the URL of your server, we'll tell you
what's vulnerable)
It can act as a testing toolkit for ShellShock for researchers as well!

### How do I use it?
ShellShocker has two different ways of being run:
* a command line utility, and
* a web interface **which will be publicly deployed to Heroku *today***

#### Usage of the CLI:
<pre>
Usage: shellshocker.py [OPTIONS] URL

  Test the URL `URL` for ShellShock vulnerability.

Options:
  -v, --verbose                   Make the tester more verbose for debugging
  -c, --command TEXT              Command to inject into the payload
  -p, --payload [traditional|new]
                                  Choose between the original bug and the new
                                  one
  --help                          Show this message and exit.
</pre>

### Hacking on the code
**`vagrant up`**.
In your Vagrant enviroment, everything'll be set up. If it somehow isn't...
**`vagrant provision`**.

If you're not in the virtualenv, activate it: `. env/bin/activate`.

### Authors
* Liam (ArchimedesPi)
