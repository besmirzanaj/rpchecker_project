# rpchecker for python

A sample app found at https://realpython.com/site-connectivity-checker-python/ and used
for learning some python things

# Install

Clone the repo

```
git clone git@github.com:besmirzanaj/rpchecker_project.git
```

Then install requirements with

```
pip install -r requirements.txt
```

# Running

```
python -m rpchecker -h
usage: rpchecker [-h] [-u URLs [URLs ...]] [-f FILE] [-a]

check the availability of web sites

options:
  -h, --help            show this help message and exit
  -u URLs [URLs ...], --urls URLs [URLs ...]
                        enter one or more website URLs
  -f FILE, --input-file FILE
                        read URLs from a file
  -a, --asynchronous    run the connectivity check asynchronously

$ # Synchronous execution
$ python -m rpchecker -u python.org pypi.org docs.python.org
The status of "python.org" is: "Online!" 👍
The status of "pypi.org" is: "Online!" 👍
The status of "docs.python.org" is: "Online!" 👍

$ # Asynchronous execution
$ python -m rpchecker -u python.org pypi.org docs.python.org -a
The status of "pypi.org" is: "Online!" 👍
The status of "docs.python.org" is: "Online!" 👍
The status of "python.org" is: "Online!" 👍
```