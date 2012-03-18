# gh-pages-template

### Make your github project page stylish

**NOTE:** will test these methods out. Use at your own risk for now.

## Installation

To integrate these changes into an existing repository, follow

### Check if you have a gh-pages branch

To confirm if you have an existing gh-pages branch, run the following commands in your fork:

    git fetch origin
    git branch -a

This will display the branches in your fork and the remote repository:

	D:\Code\github\shiftkey\gh-pages-template [master]> git branch -a
	* master
	  remotes/origin/gh-pages
	  remotes/origin/master

### Create the gh-pages branch

    cd {path to your repository}
    git checkout --orphan gh-pages 
    git remote add gh-pages-templates git://github.com/shiftkey/gh-pages-template.git
    git fetch gh-pages-templates
    git pull gh-pages-templates gh-pages
    git push origin gh-pages

### Add the template to an existing branch

    cd {path to your repository}
    git checkout gh-pages
    rm . -rf
    git add -u
    git commit -m "removed old version"
    git remote add gh-pages-templates git://github.com/shiftkey/gh-pages-template.git
    git fetch gh-pages-templates
    git pull gh-pages-templates gh-pages
    git push origin gh-pages

## Customisation

TODO