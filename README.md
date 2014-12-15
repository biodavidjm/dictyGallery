dictyGallery
============

***Gallery of pictures for the dictyBase***

Based on [PhotoFloat](https://github.com/zx2c4/PhotoFloat)

# Instructions

To create a new photo gallery:

* Delete the pictures from the folders `web/albums` and `web/cache`
* Add the pics to `web/albums`
* Run the python script in `scanner`: 

```
python main.py ../web/albums ../web/cache
```
Finally, a quick and dirty step: all the pictures in `cache` have to be renamed to `root-nameOfThePicture`.

### Notes about python

[`pyenv`](https://github.com/yyuu/pyenv) is recommended to manage python versions. 

***On the Mac***

* Use `brew` to install `pyenv`: `brew install pyenv`
* Add to `.bash_profile`: `eval "$(pyenv init -)"`
* Install a python version `pyenv install 2.7.3`
* Install the Python Imaging Library: `pip install Pillow`
* Create a `.python-version` file specifying the version version wished to be run in that folder (e.g., `2.7.3`)

