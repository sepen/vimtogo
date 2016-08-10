# ViM To Go

Deploy your custom ViM setup and keep it up to date everywhere.


### Quickstart

Installation:
```
git clone https://github.com/sepen/vimtogo
cd vimtogo
chmod +x vimtogo
./vimtogo install
```

Options:
```
Usage: ./vimtogo [install|update] <option>
Where options for commands are:
  install
  -k, --ssl-no-verify   No verify SSL certs for HTTPS connections
  -f, --force           Force installation. This will overwrite exinting files
  -b, --backup          Save existing stuff by renaming to .bk extension
```

### Customize your setup

My idea is to keep in _master_ branch the most common setup and have a branch for each customization.
In this way, you can fork my repository and create one branch that meets your needs.  
Then from time to time you can merge from this upstream repository to your fork.  
If you need more help about that take a look of this link:  
<https://help.github.com/articles/merging-an-upstream-repository-into-your-fork/>
