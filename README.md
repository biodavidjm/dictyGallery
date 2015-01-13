dictyGallery
============

***Gallery of pictures for the dictyBase***

Based on [PhotoFloat](https://github.com/zx2c4/PhotoFloat)

# Instructions

To add a new conference photo album, follow these steps:

* Add the conference photos into a folder and name it `dicty##` (`##` being the year of the dicty meeting)
* Move the folder into `web/albums/`
* go to the folder `dictyGallery/scanner/` and run the following script...:
```
python main.py ../web/albums ../web/cache
```
* Sync the folder `web/` with testdb and prod


### Notes about python

[`pyenv`](https://github.com/yyuu/pyenv) is recommended to manage python versions. 

***On the Mac***

* Use `brew` to install `pyenv`: `brew install pyenv`
* Add to `.bash_profile`: `eval "$(pyenv init -)"`
* Install a python version `pyenv install 2.7.3`
* Install the Python Imaging Library: `pip install Pillow`
* Create a `.python-version` file specifying the version version wished to be run in that folder (e.g., `2.7.3`)

