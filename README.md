dictyGallery
============

***Gallery of pictures for the dictyBase***

Based on [PhotoFloat](https://github.com/zx2c4/PhotoFloat)

# Instructions

To create a new photo gallery:

* Add all the pictures of the new dicty conference into a folder and name it `dicty##` (`##` being the year of the dicty meeting)
* Move the folder into `web/albums`
* Run in `scanner` the python script...:

```
python main.py ../web/albums ../web/cache
```

* Delete the file `root.json` from `cache`
* Copy in the server:
	* The folder `dicty##` into the folder in the server `album`
	* All the generated pictures of `cache` into the `cache` folder of the server
* Add the new album in the `root.json` file of the server, i.e.,

```
{
	"path": "", 
	"albums": [
	{"date": "Aug 2011", "path": "dicty11"},
	{"date": "Aug 2012", "path": "dicty12"}, 
	{"date": "Aug 2013", "path": "dicty13"},
	{"date": "Month ####", "path": "dicty##"} <---- This is the new album
	], 
	"photos": []
}
```


### Notes about python

[`pyenv`](https://github.com/yyuu/pyenv) is recommended to manage python versions. 

***On the Mac***

* Use `brew` to install `pyenv`: `brew install pyenv`
* Add to `.bash_profile`: `eval "$(pyenv init -)"`
* Install a python version `pyenv install 2.7.3`
* Install the Python Imaging Library: `pip install Pillow`
* Create a `.python-version` file specifying the version version wished to be run in that folder (e.g., `2.7.3`)

