# My developer handbook

## Installation

```
python3 -m venv p3venv
source p3venv/bin/activate
``` 

with the virtualenv activated:

```
pip install -r requirements.txt 
```

## Develop

```
cd docs
make clean
make html
```

## Use

go to docs/build/html and run `index.html` in a browser of your choice
