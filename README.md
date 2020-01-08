<p align="center">
  <div style='background-size: 100%; height: 200px; width: 200px; background-image: url("data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9JzMwMHB4JyB3aWR0aD0nMzAwcHgnICBmaWxsPSIjMDAwMDAwIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCIgeD0iMHB4IiB5PSIwcHgiPjxnPjxwYXRoIGQ9Ik0xNC44MTYsNEEzLDMsMCwwLDAsMTIsMkgxMEEzLDMsMCwwLDAsNyw1VjU3YTUuMDA2LDUuMDA2LDAsMCwwLDUsNUg1N1YzNmg0VjI4SDU3VjI2aDRWMThINTdWMTZoNFY4SDU3VjRaTTksNWExLDEsMCwwLDEsMS0xaDJhMSwxLDAsMCwxLDEsMVY0NEg5Wk0yMiw2MFY1NGg0djZabTMzLThINDZ2Mmg5djJIMjhWNTRoOVY1MkgxNXYyaDV2MkgxNGExLDEsMCwwLDEtMS0xVjUxYTEsMSwwLDAsMSwxLTFINTVabTAsOEgyOFY1OEg1NVptMC0xMkgxNGEzLDMsMCwwLDAtMywzdjRhMywzLDAsMCwwLDMsM2g2djJIMTJhMywzLDAsMCwxLTMtM1Y0Nkg1NVptNC0xOHY0SDU3VjMwWm0wLTEwdjRINTdWMjBaTTU1LDQ0SDE1VjZINTVabTQtMzR2NEg1N1YxMFoiPjwvcGF0aD48cmVjdCB4PSIzOSIgeT0iNTIiIHdpZHRoPSIyIiBoZWlnaHQ9IjIiPjwvcmVjdD48cGF0aCBkPSJNMTcsMzZINTNWMTRIMTdabTItMjBINTFWMzRIMTlaIj48L3BhdGg+PHBhdGggZD0iTTI1LjIxOSwxOCwyMi4wMywzMC43NThsMS45NC40ODRMMjUuMjgxLDI2aDUuNDM4bDEuMzExLDUuMjQyLDEuOTQtLjQ4NEwzMC43ODEsMThabS41NjIsNiwxLTRoMi40MzhsMSw0WiI+PC9wYXRoPjxwYXRoIGQ9Ik00NSwyMUgzN3YyaDZ2MkgzN3Y2SDQ3VjI5SDQ1Wm0tMiw4SDM5VjI3aDRaIj48L3BhdGg+PHBvbHlnb24gcG9pbnRzPSIxOSAxMCAyMyAxMCAyMyA4IDE3IDggMTcgMTIgMTkgMTIgMTkgMTAiPjwvcG9seWdvbj48cmVjdCB4PSI1MSIgeT0iOCIgd2lkdGg9IjIiIGhlaWdodD0iMiI+PC9yZWN0PjwvZz48L3N2Zz4=");'></div>
</p>

<h1 align="center">aglfn</h1>

<p align="center">
  <a href="https://travis-ci.com/puria/aglfn">
    <img src="https://travis-ci.com/puria/aglfn.svg?branch=master" alt="Build Status">
  </a>
  <a href="https://codecov.io/gh/puria/aglfn">
    <img src="https://codecov.io/gh/puria/aglfn/branch/master/graph/badge.svg" alt="Code coverage"/>
  </a>
  <a href="https://pypi.org/project/aglfn/">
    <img alt="PyPI release" src="https://img.shields.io/pypi/v/aglfn.svg" alt="Latest release">
  </a>
</p>

<div align="center"><sub>Python utilities for AGLFN (Adobe Glyph List For New Fonts) </sub></div>

<br><br>

<div align="center">
  <pre>pip install <a href="http://pypi.org/project/aglfn">aglfn</a></pre>
</div>

<br><br>


<h4 align="center">
  <a href="#-install">💾 Install</a>
  <span> • </span>
  <a href="#-quick-start">🎮 Quick start</a>
  <span> • </span>
  <a href="#-testing">📋 Testing</a>
  <span> • </span>
  <a href="#-acknowledgements">😍 Acknowledgements</a>
  <span> • </span>
  <a href="#-contributing">👤 Contributing</a>
  <span> • </span>
  <a href="#-license">💼 License</a>
</h4>


Access [AGLFN](https://github.com/adobe-type-tools/agl-aglfn) names easily in Python.



<details>
 <summary><strong>🚩 Table of Contents</strong> (click to expand)</summary>

* [Install](#-install)
* [Quick start](#-quick-start)
* [Testing](#-testing)
* [Acknowledgements](#-acknowledgements)
* [Contributing](#-contributing)
* [License](#-license)
</details>

***
## 💾 Install
```pip install aglfn```

or if you want to install it locally for development clone this repo and then

```bash
cd aglfn
pip install -e .
```

***
## 🎮 Quick start

### `names`
get the list of all the AGLFN names

```python
import aglfn

print(aglfn.names)
```

### `glyphs`
get the list of all glyphs with a corresponding AGLFN name
```python
import aglfn

print(aglfn.glyphs)
```

### `name()`
get the corresponding AGLFN name by passing a glyph
```python
import aglfn

name = aglfn.name('€')
assert 'Euro' == name
```

### `to_glyph()`
get the corresponding glyph by passing an AGLFN name
```python
import aglfn

glyph = aglfn.to_glyph('Euro')
assert '€' == glyph
```

***

## 📋 Testing

Test are executed with travis, in case you want to run them locally just:

```bash
cd aglfn
python setup.py test
```

***
## 😍 Acknowledgements

Copyright 🄯 2020 Puria Nafisi Azizi, Italy

Designed, written and maintained by Puria Nafisi Azizi.

Logo, dictionary by Smalllike from the Noun Project.


***
## 👤 Contributing

1.  🔀 [FORK IT](../../fork)
2.  Create your feature branch `git checkout -b feature/branch`
3.  Commit your changes `git commit -am 'Add some foobar'`
4.  Push to the branch `git push origin feature/branch`
5.  Create a new Pull Request
6.  🙏 Thank you


***
## 💼 License
    aglfn - Python utilities for Adobe Glyph List For New Fonts
    Copyright 🄯 2020 Puria Nafisi Azizi, Italy

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

