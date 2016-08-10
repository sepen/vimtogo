# ViM To Go

Deploy your custom ViM setup and keep it up to date everywhere.


## Quickstart

### Installation
```
git clone https://github.com/sepen/vimtogo
cd vimtogo
chmod +x vimtogo
./vimtogo install
```

### Usage
```
Usage: ./vimtogo [install|update] <option>
Where options for commands are:
  install
  -k, --ssl-no-verify   No verify SSL certs for HTTPS connections
  -f, --force           Force installation. This will overwrite exinting files
  -b, --backup          Save existing stuff by renaming to .bk extension
```

### Install more plugins

For example to add _vim-airline_ plugin to your setup:
```
vim togo/vim-airline
```
Then put these contents:
```
""" vim-airline
""" https://github.com/vim-airline/vim-airline
let g:airline#extensions#tabline#enabled=1
```
At least you have to put the first two lines which are required:
* first line indicates the plugin name
* second one referes to git repo location from where clone and or update sources

After that you can add all desired option settings. For example:
```
let g:airline#extensions#tabline#enabled=1
```

Then run the installation again that will re-install all default plugins and will add _vim-airline_:
```
./vimtogo install --force
```

To have an example of a complete setup take a look of my own branch:  
<https://github.com/sepen/vimtogo/blob/sepen/togo/>


## Customization

My idea is to keep in _master_ branch the most common setup and have a branch for each customization.
In this way, you can fork my repository and create one branch that meets your needs.  
Then from time to time you can merge from this upstream repository to your fork.  
  
If you need more help about how to merge upstream changes that take a look of this link:  
<https://help.github.com/articles/merging-an-upstream-repository-into-your-fork/>
