[![Build Status](https://travis-ci.org/martinghunt/travisty.svg?branch=master)](https://travis-ci.org/martinghunt/travisty)

# travisty
Silly repo for testing travis, CI/D, etc.


## Tests

Run `tox`. (`pip3 install tox` first, if needed.)

## pyinstaller

Create a freeze that can be run on OSX:

    pyinstaller --additional-hooks-dir=pyinstaller_hooks/ travisty/__main__.py  --name travisty --workpath=build/pyinstaller_work --distpath=build

That makes `build/travisty/`, which is self-contained directory that includes
the executable `travisty` and should run on any Mac (without Python being
installed).

