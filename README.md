# Simple Page-serving WebServer #

* This is a project for uoregon CIS 322.

### Author: Freddie Wang ###

* Email: nwang@uoregon.edu

### Features & Specifics ###

* The webserver will serve __only__ *html* and *css* files.
* All pages should be stored in *./pages/* directory to be correctly served.
* The server support following status upon each connection:
 * 200 - Everything is OK
 * 401 - Not implemented
 * 403 - Forbidden (if the url contains '//', '..', or '~' or if the page you are trying to reach is not a html or css page)
 * 404 - Not found

### Deployment ###
* The default webserver port is 8000.
* You may want to edit CONFIG.py to change port.
```bash
git clone https://github.com/TsFreddie/proj-pageserver
cd proj-pageserver
make configure
make run
```

### Testing ###
* The default testing shell script is provided in ./test/ directory.
* The test need to be able to fetch *trivia.html* and *trivia.css* to behave as intended.
* __You can modify the *tests.sh* file to suit specific testing needs.__
```bash
./tests.sh http://127.0.0.1:8000
```
