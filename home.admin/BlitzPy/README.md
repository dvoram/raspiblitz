# BlitzPy

BlitzPy is a part of the RaspiBlitz project and implements a few common use cases.


## Installation

### Prerequisite

None

### Dependencies

None

### Install BlitzPy

```
cd ~/raspiblitz/home.admin/BlitzPy
pip install dist/BlitzPy-0.1.0-py2.py3-none-any.whl
OR
sudo -H python -m pip install dist/BlitzPy-0.1.0-py2.py3-none-any.whl
```

**or** consider using a virtual environment

```
python3 -m venv --system-site-packages venv
source venv/bin/activate
pip install BlitzPy
```

## Installation

Import and use..

```
from blitzpy import RaspiBlitzConfig
cfg = RaspiBlitzConfig()
cfg.reload()
print(cfg.__dict__)
print(cfg.hostname)
if cfg.run_behind_tor:
    print("using TOR!")
```

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)