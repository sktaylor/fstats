# fstats - a file tree stats program

### Installation

Please read the section on global installation.

```
npm install -g fstats 
```

### Use (it's really easy)

just run:

`fstats [some_directory]` if you don't provide a directory, fstats will use the current working directory.

`fstats -ro [some_directory]` prevents fstats from reading or writing history in the working directory.

`fstats -h` get's some terse help.

A file `.fstats.json` will be created in the working, every time you run it the new stats will be apended to the top, and a summary will be printed to the console. The summary looks like this:

```
              current   last  change    max  change
size:           41.9M  38.0M    4.0M  43.9M   -2.0M
files:          2,921  2,907      14  2,911      10
links:             16     22      -6     23      -7
dirs:             634    633       1    634       0
files / dir:     4.58   4.59       0   4.63   -0.04
```

#### Global Installation

You should be installing "globally" to your home directory without sudo:

Run this command: ```npm config set prefix ~/.npm-packages```

Add this to your .bashrc or similar: ```export PATH=$HOME/.npm-packages/bin:$PATH```

### Contributing

Fork, add issues, send pull requests, whatever.

Apache License -- see the LICENSE file in the root of the repo for license information.
