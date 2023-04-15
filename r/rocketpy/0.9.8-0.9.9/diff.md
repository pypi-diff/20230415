# Comparing `tmp/rocketpy-0.9.8.tar.gz` & `tmp/rocketpy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketpy-0.9.8.tar", last modified: Tue Aug 24 22:20:35 2021, max compression
+gzip compressed data, was "rocketpy-0.9.9.tar", last modified: Sat Jan  8 23:10:02 2022, max compression
```

## Comparing `rocketpy-0.9.8.tar` & `rocketpy-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-08-24 22:20:35.258925 rocketpy-0.9.8/
--rw-rw-rw-   0        0        0     1079 2021-08-20 18:47:30.000000 rocketpy-0.9.8/LICENSE
--rw-rw-rw-   0        0        0    12111 2021-08-24 22:20:35.257928 rocketpy-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0    11218 2021-08-20 18:47:30.000000 rocketpy-0.9.8/README.md
--rw-rw-rw-   0        0        0        0 2021-08-24 20:53:14.000000 rocketpy-0.9.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2021-08-24 22:20:35.215043 rocketpy-0.9.8/rocketpy/
--rw-rw-rw-   0        0        0   143383 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/Environment.py
--rw-rw-rw-   0        0        0   150306 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/Flight.py
--rw-rw-rw-   0        0        0    88272 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/Function.py
--rw-rw-rw-   0        0        0    40263 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/Rocket.py
--rw-rw-rw-   0        0        0    29417 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/SolidMotor.py
--rw-rw-rw-   0        0        0     1446 2021-08-20 18:47:30.000000 rocketpy-0.9.8/rocketpy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-24 22:20:35.254935 rocketpy-0.9.8/rocketpy.egg-info/
--rw-rw-rw-   0        0        0    12111 2021-08-24 22:20:35.000000 rocketpy-0.9.8/rocketpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2021-08-24 22:20:35.000000 rocketpy-0.9.8/rocketpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-24 22:20:35.000000 rocketpy-0.9.8/rocketpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2021-08-24 22:20:35.000000 rocketpy-0.9.8/rocketpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-08-24 22:20:35.000000 rocketpy-0.9.8/rocketpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-24 22:20:35.259923 rocketpy-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      849 2021-08-20 18:47:30.000000 rocketpy-0.9.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2022-01-08 23:09:08.000000 rocketpy-0.9.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13285 2022-01-08 23:10:02.237356 rocketpy-0.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12744 2022-01-08 23:09:08.000000 rocketpy-0.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/rocketpy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   143398 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Environment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150672 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Flight.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88141 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41975 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Rocket.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29902 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/SolidMotor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/utilities.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/rocketpy.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13285 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-01-08 23:10:02.237356 rocketpy-0.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      808 2022-01-08 23:09:11.000000 rocketpy-0.9.9/setup.py
```

### Comparing `rocketpy-0.9.8/LICENSE` & `rocketpy-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketpy-0.9.8/PKG-INFO` & `rocketpy-0.9.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,352 +1,344 @@
-Metadata-Version: 2.1
-Name: rocketpy
-Version: 0.9.8
-Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/giovaniceotto/RocketPy
-Author: Giovani Hidalgo Ceotto
-Author-email: ghceotto@gmail.com
-Maintainer: RocketPy Developers
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://rocketpyalpha.readthedocs.io/en/latest/?badge=latest)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)
-[![Downloads](https://pepy.tech/badge/rocketpyalpha)](https://pepy.tech/project/rocketpyalpha)
-[![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
-
-# RocketPy
-RocketPy is a trajectory simulation for High-Power Rocketry built by [Projeto Jupiter](https://www.facebook.com/ProjetoJupiter/). The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
-
-### Main features
-
-<details>
-<summary>Nonlinear 6 degrees of freedom simulations</summary>
-<ul>
-  <li>Rigorous treatment of mass variation effects</li>
-  <li>Solved using LSODA with adjustable error tolerances</li>
-  <li>Highly optimized to run fast</li>
-</ul>
-</details>
-
-<details>
-<summary>Accurate weather modeling</summary>
-<ul>
-  <li>International Standard Atmosphere (1976)</li>
-  <li>Custom atmospheric profiles</li>
-  <li>Soundings (Wyoming, NOAARuc)</li>
-  <li>Weather forecasts and reanalysis</li>
-  <li>Weather ensembles</li>
-</ul>
-</details>
-
-<details>
-<summary>Aerodynamic models</summary>
-<ul>
-  <li>Barrowman equations for lift coefficients (optional)</li>
-  <li>Drag coefficients can be easily imported from other sources (e.g. CFD simulations)</li>
-</ul>
-</details>
-
-<details>
-<summary>Parachutes with external trigger functions</summary>
-<ul>
-  <li>Test the exact code that will fly</li>
-  <li>Sensor data can be augmented with noise</li>
-</ul>
-</details>
-
-<details>
-<summary>Solid motors models</summary>
-<ul>
-  <li>Burn rate and mass variation properties from thrust curve</li>
-  <li>CSV and ENG file support</li>
-</ul>
-</details>
-
-<details>
-<summary>Monte Carlo simulations</summary>
-<ul>
-  <li>Dispersion analysis</li>
-  <li>Global sensitivity analysis</li>
-</ul>
-</details>
-
-<details>
-<summary>Flexible and modular</summary>
-<ul>
-  <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
-  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
-  <li>Multi-stage rockets</li>
-  <li>Custom continuous and discrete control laws</li>
-  <li>Create new classes (e.g. other types of motors)</li>
-</ul>
-</details>
-
-### Documentation
-
-Check out documentation details using the links below:
-  - [User Guide](https://rocketpyalpha.readthedocs.io/en/latest/user/index.html)
-  - [Code Documentation](https://rocketpyalpha.readthedocs.io/en/latest/reference/index.html)
-  - [Development Guide](https://rocketpyalpha.readthedocs.io/en/latest/development/index.html)
-
-## Join Our Community!
-RocketPy is growing fast! Many unviersity groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
-
-If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
-
-## Previewing
-
-You can preview RocketPy's main functionalities by browsing through a sample notebook either in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb) or in [MyBinder](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)!
-
-Then, you can read the *Getting Started* section to get your own copy!
-
-## Getting Started
-
-These instructions will get you a copy of RocketPy up and running on your local machine.
-
-### Prerequisites
-
-The following is needed in order to run RocketPy:
-
- - Python >= 3.0
- - Numpy >= 1.0
- - Scipy >= 1.0
- - Matplotlib >= 3.0
- - requests
- - netCDF4 >= 1.4 (optional, requires Cython)
- 
-All of these packages, with the exception of netCDF4, should be automatically
-installed when RocketPy is installed using either pip or conda.
-
-However, in case the user wants to install these packages manually, they can do
-so by following the instructions bellow:
-
-The first 4 prerequisites come with Anaconda, but Scipy might need
-updating. The nedCDF4 package can be installed if there is interest in
-importing weather data from netCDF files. To update Scipy and install
-netCDF4 using Conda, the following code is used:
-
-```
-$ conda install "scipy>=1.0"
-$ conda install -c anaconda "netcdf4>=1.4"
-```
-
-Alternatively, if you only have Python 3.X installed, the packages needed can be installed using pip:
-
-```
-$ pip install "numpy>=1.0"
-$ pip install "scipy>=1.0"
-$ pip install "matplotlib>=3.0"
-$ pip install "netCDF4>=1.4"
-$ pip install "requests"
-```
-
-Although [Jupyter Notebooks](http://jupyter.org/) are by no means required to run RocketPy, they are strongly recommend. They already come with Anaconda builds, but can also be installed separately using pip:
-
-```
-$ pip install jupyter
-```
-
-### Installation
-
-To get a copy of RocketPy using pip, just run:
-
-```
-$ pip install rocketpyalpha
-```
-
-Alternatively, the package can also be installed using conda:
-
-```
-$ conda install -c conda-forge rocketpy
-```
-
-If you want to downloaded it from source, you may do so either by:
-
-- Downloading it from [RocketPy's GitHub](https://github.com/giovaniceotto/RocketPy) page
-    - Unzip the folder and you are ready to go
-- Or cloning it to a desired directory using git:
-    - ```$ git clone https://github.com/giovaniceotto/RocketPy.git```
-
-The RockeyPy library can then be installed by running:
-
-```
-$ python setup.py install 
-```
-
-### Documentations
-
-You can find RocketPy's documentation at [Read the Docs](https://rocketpyalpha.readthedocs.io/en/latest/).
-
-### Running Your First Simulation
-
-In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the **_nbks_** folder. Open **_Getting Started - Examples.ipynb_** and you are ready to go.
-
-Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
-
-- Environment - Keeps data related to weather.
-- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
-- Rocket - Keeps data related to a rocket.
-- Flight - Runs the simulation and keeps the results.
-
-A typical workflow starts with importing these classes from RocketPy:
-
-```python
-from rocketpy import Environment, Rocket, SolidMotor, Flight
-```
-
-Then create an Environment object. To learn more about it, you can use:
-
-```python
-help(Environment)
-```
-
-A sample code is:
-
-```python
-Env = Environment(
-    railLength=5.2,
-    latitude=32.990254,
-    longitude=-106.974998,
-    elevation=1400,
-    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
-) 
-
-Env.setAtmosphericModel(type='Forecast', file='GFS')
-```
-
-This can be followed up by starting a Solid Motor object. To get help on it, just use:
-
-```python
-help(SolidMotor)
-```
-
-A sample Motor object can be created by the following code:
-
-```python
-Pro75M1670 = SolidMotor(
-    thrustSource="../data/motors/Cesaroni_M1670.eng",
-    burnOut=3.9,
-    grainNumber=5,
-    grainSeparation=5/1000,
-    grainDensity=1815,
-    grainOuterRadius=33/1000,
-    grainInitialInnerRadius=15/1000,
-    grainInitialHeight=120/1000,
-    nozzleRadius=33/1000,
-    throatRadius=11/1000,
-    interpolationMethod='linear'
-)
-```
-
-With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
-
-```python
-help(Rocket)
-```
-
-A sample code to create a Rocket is:
-
-```python
-Calisto = Rocket(
-    motor=Pro75M1670,
-    radius=127/2000,
-    mass=19.197-2.956,
-    inertiaI=6.60,
-    inertiaZ=0.0351,
-    distanceRocketNozzle=-1.255,
-    distanceRocketPropellant=-0.85704,
-    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
-    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
-)
-
-Calisto.setRailButtons([0.2, -0.5])
-
-NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
-
-FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
-
-Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
-```
-
-You may want to add parachutes to your rocket as well:
-
-```python
-def drogueTrigger(p, y):
-    return True if y[5] < 0 else False
-
-def mainTrigger(p, y):
-    return True if y[5] < 0 and y[2] < 800 else False
-
-Main = Calisto.addParachute('Main',
-                            CdS=10.0,
-                            trigger=mainTrigger, 
-                            samplingRate=105,
-                            lag=1.5,
-                            noise=(0, 8.3, 0.5))
-
-Drogue = Calisto.addParachute('Drogue',
-                              CdS=1.0,
-                              trigger=drogueTrigger, 
-                              samplingRate=105,
-                              lag=1.5,
-                              noise=(0, 8.3, 0.5))
-```
-
-Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
-
-```python
-help(Flight)
-```
-
-To actually create a Flight object, use:
-
-```python
-TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
-```
-
-Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
-
-```python
-TestFlight.info()
-```
-
-To seel all available results, use:
-
-```python
-TestFlight.allInfo()
-```
-
-## Built With
-
-* [Numpy](http://www.numpy.org/)
-* [Scipy](https://www.scipy.org/)
-* [Matplotlib](https://matplotlib.org/)
-* [netCDF4](https://github.com/Unidata/netcdf4-python)
-
-## Contributing
-
-Please read [CONTRIBUTING.md](https://github.com/giovaniceotto/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us. - **_Still working on this!_**
-
-## Authors
-
-* Creator: **Giovani Hidalgo Ceotto**
-
-See the list of [contributors](https://github.com/giovaniceotto/RocketPy/contributors) who are actively working on RocketPy.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/giovaniceotto/RocketPy/blob/master/LICENSE) file for details
-
-## Release Notes
-Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/giovaniceotto/RocketPy/releases).
-
-
-
+Metadata-Version: 2.1
+Name: rocketpy
+Version: 0.9.9
+Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
+Home-page: https://github.com/giovaniceotto/RocketPy
+Author: Giovani Hidalgo Ceotto
+Author-email: ghceotto@gmail.com
+Maintainer: RocketPy Developers
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![RocketPy Logo](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
+
+<br>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
+[![PyPI](https://img.shields.io/pypi/v/rocketpy?color=g)](https://pypi.org/project/rocketpy/)
+[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://docs.rocketpy.org/en/latest/?badge=latest)
+[![Build Status](https://app.travis-ci.com/Projeto-Jupiter/RocketPy.svg?branch=master)](https://app.travis-ci.com/Projeto-Jupiter/RocketPy)
+[![Contributors](https://img.shields.io/github/contributors/Projeto-Jupiter/rocketpy)](https://github.com/Projeto-Jupiter/RocketPy/graphs/contributors)
+[![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/rocketpy)
+[![DOI](https://img.shields.io/badge/DOI-10.1061%2F%28ASCE%29AS.1943--5525.0001331-blue.svg)](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331)
+
+<img src="https://static.scarf.sh/a.png?x-pxid=6f4094ab-00fa-4a8d-9247-b7ed27e7164d" />
+
+# RocketPy
+RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
+
+<br>
+
+## Main features
+<details>
+<summary>Nonlinear 6 degrees of freedom simulations</summary>
+<ul>
+  <li>Rigorous treatment of mass variation effects</li>
+  <li>Solved using LSODA with adjustable error tolerances</li>
+  <li>Highly optimized to run fast</li>
+</ul>
+</details>
+
+<details>
+<summary>Accurate weather modeling</summary>
+<ul>
+  <li>International Standard Atmosphere (1976)</li>
+  <li>Custom atmospheric profiles</li>
+  <li>Soundings (Wyoming, NOAARuc)</li>
+  <li>Weather forecasts and reanalysis</li>
+  <li>Weather ensembles</li>
+</ul>
+</details>
+
+<details>
+<summary>Aerodynamic models</summary>
+<ul>
+  <li>Barrowman equations for lift coefficients (optional)</li>
+  <li>Drag coefficients can be easily imported from other sources (e.g. CFD simulations)</li>
+</ul>
+</details>
+
+<details>
+<summary>Parachutes with external trigger functions</summary>
+<ul>
+  <li>Test the exact code that will fly</li>
+  <li>Sensor data can be augmented with noise</li>
+</ul>
+</details>
+
+<details>
+<summary>Solid motors models</summary>
+<ul>
+  <li>Burn rate and mass variation properties from thrust curve</li>
+  <li>CSV and ENG file support</li>
+</ul>
+</details>
+
+<details>
+<summary>Monte Carlo simulations</summary>
+<ul>
+  <li>Dispersion analysis</li>
+  <li>Global sensitivity analysis</li>
+</ul>
+</details>
+
+<details>
+<summary>Flexible and modular</summary>
+<ul>
+  <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
+  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
+  <li>Multi-stage rockets</li>
+  <li>Custom continuous and discrete control laws</li>
+  <li>Create new classes (e.g. other types of motors)</li>
+</ul>
+</details>
+
+<br>
+
+## Validation
+
+RocketPy's features have been validated in our latest [research article published in the Journal of Aerospace Engineering](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331).
+
+The table below shows a comparison between experimental data and the output from RocketPy.
+Flight data and rocket parameters used in this comparison were kindly provided by [EPFL Rocket Team](https://github.com/EPFLRocketTeam) and [Notre Dame Rocket Team](https://ndrocketry.weebly.com/).
+
+|         Mission         |    Result Paramater    | RocketPy  | Measured  | Relative Error |
+|:-----------------------:|:-----------------------|:---------:|:---------:|:--------------:|
+|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**   |
+|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**   |
+|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **4.24 %**   |
+|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**  |
+|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**  |
+|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**   |
+
+<br>
+
+## Documentation
+
+Check out documentation details using the links below:
+
+  - [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
+  - [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
+  - [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
+
+<br>
+
+# Join Our Community!
+RocketPy is growing fast! Many university groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
+
+If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
+
+<br>
+
+# Previewing
+
+You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb).  No installation required!
+
+When you are ready to run RocketPy locally, you can read the *Getting Started* section!
+
+<br>
+
+# Getting Started
+
+## Quick Installation
+
+To install RocketPy's latest stable version from PyPI, just open up your terminal and run:
+
+```shell
+pip install rocketpy
+```
+
+For other installation options, visit our [Installation Docs](https://docs.rocketpy.org/en/latest/user/installation.html).
+To learn more about RocketPy's requirements, visit our [Requirements Docs](https://docs.rocketpy.org/en/latest/user/requirements.html).
+
+<br>
+
+## Running Your First Simulation
+
+In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _nbks_ folder. Open _Getting Started - Examples.ipynb_ and you are ready to go.
+
+Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
+
+- Environment - Keeps data related to weather.
+- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
+- Rocket - Keeps data related to a rocket.
+- Flight - Runs the simulation and keeps the results.
+
+The following image shows how the four main classes interact with each other:
+
+![Diagram](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
+
+A typical workflow starts with importing these classes from RocketPy:
+
+```python
+from rocketpy import Environment, Rocket, SolidMotor, Flight
+```
+
+Then create an Environment object. To learn more about it, you can use:
+
+```python
+help(Environment)
+```
+
+A sample code is:
+
+```python
+Env = Environment(
+    railLength=5.2,
+    latitude=32.990254,
+    longitude=-106.974998,
+    elevation=1400,
+    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
+) 
+
+Env.setAtmosphericModel(type='Forecast', file='GFS')
+```
+
+This can be followed up by starting a Solid Motor object. To get help on it, just use:
+
+```python
+help(SolidMotor)
+```
+
+A sample Motor object can be created by the following code:
+
+```python
+Pro75M1670 = SolidMotor(
+    thrustSource="../data/motors/Cesaroni_M1670.eng",
+    burnOut=3.9,
+    grainNumber=5,
+    grainSeparation=5/1000,
+    grainDensity=1815,
+    grainOuterRadius=33/1000,
+    grainInitialInnerRadius=15/1000,
+    grainInitialHeight=120/1000,
+    nozzleRadius=33/1000,
+    throatRadius=11/1000,
+    interpolationMethod='linear'
+)
+```
+
+With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
+
+```python
+help(Rocket)
+```
+
+A sample code to create a Rocket is:
+
+```python
+Calisto = Rocket(
+    motor=Pro75M1670,
+    radius=127/2000,
+    mass=19.197-2.956,
+    inertiaI=6.60,
+    inertiaZ=0.0351,
+    distanceRocketNozzle=-1.255,
+    distanceRocketPropellant=-0.85704,
+    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
+    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
+)
+
+Calisto.setRailButtons([0.2, -0.5])
+
+NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
+
+FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
+
+Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
+```
+
+You may want to add parachutes to your rocket as well:
+
+```python
+def drogueTrigger(p, y):
+    return True if y[5] < 0 else False
+
+def mainTrigger(p, y):
+    return True if y[5] < 0 and y[2] < 800 else False
+
+Main = Calisto.addParachute('Main',
+                            CdS=10.0,
+                            trigger=mainTrigger, 
+                            samplingRate=105,
+                            lag=1.5,
+                            noise=(0, 8.3, 0.5))
+
+Drogue = Calisto.addParachute('Drogue',
+                              CdS=1.0,
+                              trigger=drogueTrigger, 
+                              samplingRate=105,
+                              lag=1.5,
+                              noise=(0, 8.3, 0.5))
+```
+
+Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
+
+```python
+help(Flight)
+```
+
+To actually create a Flight object, use:
+
+```python
+TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
+```
+
+Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
+
+```python
+TestFlight.info()
+```
+
+To seel all available results, use:
+
+```python
+TestFlight.allInfo()
+```
+
+Here is just a quick taste of what RocketPy is able to calculate. There are hundred of plots and data points computed by RocketPy to enhance your analyses.
+
+![6-DOF Trajectory Plot](docs/static/rocketpy_example_trajectory.svg)
+
+<br>
+
+# Authors and Contributors
+
+This package was originally created by [Giovani Ceotto](https://github.com/giovaniceotto/) as part of his work at [Projeto Jupiter](https://github.com/Projeto-Jupiter/). [Rodrigo Schmitt](https://github.com/rodrigo-schmitt/) was one of the first contributors.
+
+Later, [Guilherme Fernandes](https://github.com/Gui-FernandesBR/) and [Lucas Azevedo](https://github.com/lucasfourier/) joined the team to work on the expansion and sustainability of this project.
+
+Since then, the [RocketPy Team](https://github.com/orgs/Projeto-Jupiter/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
+
+[![GitHub Contributors Image](https://contrib.rocks/image?repo=Projeto-Jupiter/RocketPy)](https://github.com/Projeto-Jupiter/RocketPy/contributors)
+
+See a [detailed list of contributors](https://github.com/Projeto-Jupiter/RocketPy/contributors) who are actively working on RocketPy.
+
+## Supporting RocketPy and Contributing
+
+The easiest way to help RocketPy is to demonstrate your support by starring our repository! ![GitHub Repo stars](https://img.shields.io/github/stars/Projeto-Jupiter/RocketPy?style=social)
+
+<br>
+
+If you are actively using RocketPy in one of your projects, reaching out to our core team via [Discord](https://discord.gg/b6xYnNh) and providing feedback can help improve RocketPy a lot!
+
+And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more on how you can contribute with the development of this next-gen trajectory simulation solution for rocketry.
+
+<br>
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/LICENSE) file for details
+
+<br>
+
+## Release Notes
+Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/Projeto-Jupiter/RocketPy/releases).
+
+
```

### Comparing `rocketpy-0.9.8/README.md` & `rocketpy-0.9.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
-[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://rocketpyalpha.readthedocs.io/en/latest/?badge=latest)
+![RocketPy Logo](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
+
+<br>
+
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)
-[![Downloads](https://pepy.tech/badge/rocketpyalpha)](https://pepy.tech/project/rocketpyalpha)
+[![PyPI](https://img.shields.io/pypi/v/rocketpy?color=g)](https://pypi.org/project/rocketpy/)
+[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://docs.rocketpy.org/en/latest/?badge=latest)
+[![Build Status](https://app.travis-ci.com/Projeto-Jupiter/RocketPy.svg?branch=master)](https://app.travis-ci.com/Projeto-Jupiter/RocketPy)
+[![Contributors](https://img.shields.io/github/contributors/Projeto-Jupiter/rocketpy)](https://github.com/Projeto-Jupiter/RocketPy/graphs/contributors)
 [![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/rocketpy)
+[![DOI](https://img.shields.io/badge/DOI-10.1061%2F%28ASCE%29AS.1943--5525.0001331-blue.svg)](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331)
+
+<img src="https://static.scarf.sh/a.png?x-pxid=6f4094ab-00fa-4a8d-9247-b7ed27e7164d" />
 
 # RocketPy
-RocketPy is a trajectory simulation for High-Power Rocketry built by [Projeto Jupiter](https://www.facebook.com/ProjetoJupiter/). The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
+RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
 
-### Main features
+<br>
 
+## Main features
 <details>
 <summary>Nonlinear 6 degrees of freedom simulations</summary>
 <ul>
   <li>Rigorous treatment of mass variation effects</li>
   <li>Solved using LSODA with adjustable error tolerances</li>
   <li>Highly optimized to run fast</li>
 </ul>
@@ -68,121 +78,89 @@
   <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
   <li>Multi-stage rockets</li>
   <li>Custom continuous and discrete control laws</li>
   <li>Create new classes (e.g. other types of motors)</li>
 </ul>
 </details>
 
-### Documentation
-
-Check out documentation details using the links below:
-  - [User Guide](https://rocketpyalpha.readthedocs.io/en/latest/user/index.html)
-  - [Code Documentation](https://rocketpyalpha.readthedocs.io/en/latest/reference/index.html)
-  - [Development Guide](https://rocketpyalpha.readthedocs.io/en/latest/development/index.html)
-
-## Join Our Community!
-RocketPy is growing fast! Many unviersity groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
-
-If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
-
-## Previewing
-
-You can preview RocketPy's main functionalities by browsing through a sample notebook either in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb) or in [MyBinder](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)!
+<br>
 
-Then, you can read the *Getting Started* section to get your own copy!
+## Validation
 
-## Getting Started
+RocketPy's features have been validated in our latest [research article published in the Journal of Aerospace Engineering](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331).
 
-These instructions will get you a copy of RocketPy up and running on your local machine.
+The table below shows a comparison between experimental data and the output from RocketPy.
+Flight data and rocket parameters used in this comparison were kindly provided by [EPFL Rocket Team](https://github.com/EPFLRocketTeam) and [Notre Dame Rocket Team](https://ndrocketry.weebly.com/).
 
-### Prerequisites
+|         Mission         |    Result Paramater    | RocketPy  | Measured  | Relative Error |
+|:-----------------------:|:-----------------------|:---------:|:---------:|:--------------:|
+|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**   |
+|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**   |
+|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **4.24 %**   |
+|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**  |
+|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**  |
+|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**   |
 
-The following is needed in order to run RocketPy:
+<br>
 
- - Python >= 3.0
- - Numpy >= 1.0
- - Scipy >= 1.0
- - Matplotlib >= 3.0
- - requests
- - netCDF4 >= 1.4 (optional, requires Cython)
- 
-All of these packages, with the exception of netCDF4, should be automatically
-installed when RocketPy is installed using either pip or conda.
+## Documentation
 
-However, in case the user wants to install these packages manually, they can do
-so by following the instructions bellow:
+Check out documentation details using the links below:
 
-The first 4 prerequisites come with Anaconda, but Scipy might need
-updating. The nedCDF4 package can be installed if there is interest in
-importing weather data from netCDF files. To update Scipy and install
-netCDF4 using Conda, the following code is used:
+  - [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
+  - [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
+  - [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
 
-```
-$ conda install "scipy>=1.0"
-$ conda install -c anaconda "netcdf4>=1.4"
-```
+<br>
 
-Alternatively, if you only have Python 3.X installed, the packages needed can be installed using pip:
+# Join Our Community!
+RocketPy is growing fast! Many university groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
 
-```
-$ pip install "numpy>=1.0"
-$ pip install "scipy>=1.0"
-$ pip install "matplotlib>=3.0"
-$ pip install "netCDF4>=1.4"
-$ pip install "requests"
-```
-
-Although [Jupyter Notebooks](http://jupyter.org/) are by no means required to run RocketPy, they are strongly recommend. They already come with Anaconda builds, but can also be installed separately using pip:
-
-```
-$ pip install jupyter
-```
+If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
 
-### Installation
+<br>
 
-To get a copy of RocketPy using pip, just run:
+# Previewing
 
-```
-$ pip install rocketpyalpha
-```
+You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb).  No installation required!
 
-Alternatively, the package can also be installed using conda:
+When you are ready to run RocketPy locally, you can read the *Getting Started* section!
 
-```
-$ conda install -c conda-forge rocketpy
-```
+<br>
 
-If you want to downloaded it from source, you may do so either by:
+# Getting Started
 
-- Downloading it from [RocketPy's GitHub](https://github.com/giovaniceotto/RocketPy) page
-    - Unzip the folder and you are ready to go
-- Or cloning it to a desired directory using git:
-    - ```$ git clone https://github.com/giovaniceotto/RocketPy.git```
+## Quick Installation
 
-The RockeyPy library can then be installed by running:
+To install RocketPy's latest stable version from PyPI, just open up your terminal and run:
 
-```
-$ python setup.py install 
+```shell
+pip install rocketpy
 ```
 
-### Documentations
+For other installation options, visit our [Installation Docs](https://docs.rocketpy.org/en/latest/user/installation.html).
+To learn more about RocketPy's requirements, visit our [Requirements Docs](https://docs.rocketpy.org/en/latest/user/requirements.html).
 
-You can find RocketPy's documentation at [Read the Docs](https://rocketpyalpha.readthedocs.io/en/latest/).
+<br>
 
-### Running Your First Simulation
+## Running Your First Simulation
 
-In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the **_nbks_** folder. Open **_Getting Started - Examples.ipynb_** and you are ready to go.
+In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _nbks_ folder. Open _Getting Started - Examples.ipynb_ and you are ready to go.
 
 Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
 
 - Environment - Keeps data related to weather.
 - SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
 - Rocket - Keeps data related to a rocket.
 - Flight - Runs the simulation and keeps the results.
 
+The following image shows how the four main classes interact with each other:
+
+![Diagram](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
+
 A typical workflow starts with importing these classes from RocketPy:
 
 ```python
 from rocketpy import Environment, Rocket, SolidMotor, Flight
 ```
 
 Then create an Environment object. To learn more about it, you can use:
@@ -303,31 +281,45 @@
 
 To seel all available results, use:
 
 ```python
 TestFlight.allInfo()
 ```
 
-## Built With
+Here is just a quick taste of what RocketPy is able to calculate. There are hundred of plots and data points computed by RocketPy to enhance your analyses.
+
+![6-DOF Trajectory Plot](docs/static/rocketpy_example_trajectory.svg)
 
-* [Numpy](http://www.numpy.org/)
-* [Scipy](https://www.scipy.org/)
-* [Matplotlib](https://matplotlib.org/)
-* [netCDF4](https://github.com/Unidata/netcdf4-python)
+<br>
 
-## Contributing
+# Authors and Contributors
 
-Please read [CONTRIBUTING.md](https://github.com/giovaniceotto/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us. - **_Still working on this!_**
+This package was originally created by [Giovani Ceotto](https://github.com/giovaniceotto/) as part of his work at [Projeto Jupiter](https://github.com/Projeto-Jupiter/). [Rodrigo Schmitt](https://github.com/rodrigo-schmitt/) was one of the first contributors.
 
-## Authors
+Later, [Guilherme Fernandes](https://github.com/Gui-FernandesBR/) and [Lucas Azevedo](https://github.com/lucasfourier/) joined the team to work on the expansion and sustainability of this project.
 
-* Creator: **Giovani Hidalgo Ceotto**
+Since then, the [RocketPy Team](https://github.com/orgs/Projeto-Jupiter/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
 
-See the list of [contributors](https://github.com/giovaniceotto/RocketPy/contributors) who are actively working on RocketPy.
+[![GitHub Contributors Image](https://contrib.rocks/image?repo=Projeto-Jupiter/RocketPy)](https://github.com/Projeto-Jupiter/RocketPy/contributors)
+
+See a [detailed list of contributors](https://github.com/Projeto-Jupiter/RocketPy/contributors) who are actively working on RocketPy.
+
+## Supporting RocketPy and Contributing
+
+The easiest way to help RocketPy is to demonstrate your support by starring our repository! ![GitHub Repo stars](https://img.shields.io/github/stars/Projeto-Jupiter/RocketPy?style=social)
+
+<br>
+
+If you are actively using RocketPy in one of your projects, reaching out to our core team via [Discord](https://discord.gg/b6xYnNh) and providing feedback can help improve RocketPy a lot!
+
+And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more on how you can contribute with the development of this next-gen trajectory simulation solution for rocketry.
+
+<br>
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/giovaniceotto/RocketPy/blob/master/LICENSE) file for details
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/LICENSE) file for details
 
-## Release Notes
-Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/giovaniceotto/RocketPy/releases).
+<br>
 
+## Release Notes
+Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/Projeto-Jupiter/RocketPy/releases).
```

### Comparing `rocketpy-0.9.8/rocketpy/Environment.py` & `rocketpy-0.9.9/rocketpy/Environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Attributes
     ----------
 
         Constants
         Environment.earthRadius : float
             Value of Earth's Radius = 6.3781e6 m.
         Environment.airGasConstant : float
-            Value of Air's Gast Constant = 287.05287 J/K/Kg
+            Value of Air's Gas Constant = 287.05287 J/K/Kg
 
         Gravity and Launch Rail Length:
         Environment.rl : float
             Launch rail length in meters.
         Environment.g : float
             Positive value of gravitational acceleration in m/s^2.
 
@@ -78,22 +78,22 @@
         Environment.initialEW: string
             Launch site E/W hemisphere
         Environment.elevation : float
             Launch site elevation.
         Environment.date : datetime
             Date time of launch.
 
-        Topographic informations:
+        Topographic information:
         Environment.elevLonArray: array
             Unidimensional array containing the longitude coordinates
         Environment.elevLatArray: array
             Unidimensional array containing the latitude coordinates
         Environment.elevArray: array
             Two-dimensional Array containing the elevation information
-        Environment.topograficProfileAticvated: bool
+        Environment.topographicProfileActivated: bool
             True if the user already set a topographic plofile
 
         Atmosphere Static Conditions:
         Environment.maxExpectedHeight : float
             Maximum altitude in meters to keep weather data.
             Used especially for plotting range.
             Can be altered as desired.
@@ -163,15 +163,15 @@
         Atmospheric Model Details
         Environment.atmosphericModelType : string
             Describes the atmospheric model which is being used.
             Can only assume the following values: 'StandardAtmosphere',
             'CustomAtmosphere', 'WyomingSounding', 'NOAARucSounding',
             'Forecast', 'Reanalysis', 'Ensemble'.
         Environment.atmosphericModelFile : string
-            Adress of the file used for the atmospheric model being used.
+            Address of the file used for the atmospheric model being used.
             Only defined for 'WyomingSounding', 'NOAARucSounding',
             'Forecast', 'Reanalysis', 'Ensemble'
         Environment.atmosphericModelDict : dictionary
             Dictionary used to properly interpret netCDF and OPeNDAP
             files. Only defined for 'Forecast', 'Reanalysis', 'Ensemble'.
         Environment.atmosphericModelInitDate : datetime
             Datetime object instance of first availabe date in netCDF
@@ -328,15 +328,15 @@
             longitude must also be specified. Default value is 0.
         datum:
 
         Returns
         -------
         None
         """
-        # Save launch rail ength
+        # Save launch rail length
         self.rL = railLength
 
         # Save gravity value
         self.g = gravity
 
         # Save datum
         self.datum = datum
@@ -500,15 +500,15 @@
         type : string
             Defines the topographic model to be used, usually 'NASADEM Merged
             DEM Global 1 arc second nc' can be used. To download this kind of
             data, access 'https://search.earthdata.nasa.gov/search'.
             NASADEM data products were derived from original telemetry data from
             the Shuttle Radar Topography Mission (SRTM).
         file : string
-            The path/name of the topografic file. Usually .nc provided by
+            The path/name of the topographic file. Usually .nc provided by
         dictionary : string, optional
             Dictionary which helps to read the specified file. By default
             'netCDF4' which works well with .nc files will be used.
         crs : string, optional
             Coordinate reference system, by default None, which will use the crs
             provided by the file.
         """
@@ -516,15 +516,15 @@
         if type == "NASADEM_HGT":
             if dictionary == "netCDF4":
                 rootgrp = Dataset(file, "r", format="NETCDF4")
                 self.elevLonArray = rootgrp.variables["lon"][:].tolist()
                 self.elevLatArray = rootgrp.variables["lat"][:].tolist()
                 self.elevArray = rootgrp.variables["NASADEM_HGT"][:].tolist()
                 # crsArray = rootgrp.variables['crs'][:].tolist().
-                self.topograficProfileAticvated = True
+                self.topographicProfileActivated = True
 
                 print("Region covered by the Topographical file: ")
                 print(
                     "Latitude from {:.6f}° to {:.6f}°".format(
                         self.elevLatArray[-1], self.elevLatArray[0]
                     )
                 )
@@ -555,15 +555,15 @@
         Raises
         ------
         ValueError
             [description]
         ValueError
             [description]
         """
-        if self.topograficProfileAticvated == False:
+        if self.topographicProfileActivated == False:
             print(
                 "You must define a Topographic profile first, please use the method Environment.setTopograghicProfile()"
             )
             return None
 
         # Find latitude index
         # Check if reversed or sorted
@@ -640,15 +640,15 @@
         wind_v=0,
     ):
         """Defines an atmospheric model for the Environment.
         Supported functionality includes using data from the
         International Standard Atmosphere, importing data from
         weather reanalysis, forecasts and ensemble forecasts,
         importing data from upper air soundings and inputing
-        data as costum functions, arrays or csv files.
+        data as custom functions, arrays or csv files.
 
         Parameters
         ----------
         type : string
             One of the following options:
             - 'StandardAtmosphere': sets pressure and temperature
             profiles corresponding to the International Standard
@@ -746,32 +746,32 @@
             or temperature is not given, it will default to the
             International Standard Atmosphere. If the wind components
             are not given, it will default to 0.
         file : string, optional
             String that must be given when type is either
             'WyomingSounding', 'Forecast', 'Reanalysis' or 'Ensemble'.
             It specifies the location of the data given, either through
-            a local file adress or a URL.
+            a local file address or a URL.
             If type is 'Forecast', this parameter can also be either
             'GFS', 'FV3', 'RAP' or 'NAM' for latest of these forecasts.
             References: GFS: Global - 0.25deg resolution - Updates every 6 hours, forecast for 81 points spaced by 3 hours
                         FV3: Global - 0.25deg resolution - Updates every 6 hours, forecast for 129 points spaced by 3 hours
                         RAP: Regional USA - 0.19deg resolution - Updates hourly, forecast for 40 points spaced hourly
                         NAM: Regional CONUS Nest - 5 km resolution - Updates every 6 hours, forecast for 21 points spaced by 3 hours
             If type is 'Ensemble', this parameter can also be either
             'GEFS', or 'CMC' for the latest of these ensembles.
-            Refrences: GEFS: Global, bias-corrected, 0.5deg resolution, 21 forecast members, Updates every 6 hours, forecast for 65 points spaced by 4 hours
+            References: GEFS: Global, bias-corrected, 0.5deg resolution, 21 forecast members, Updates every 6 hours, forecast for 65 points spaced by 4 hours
                        CMC: Global, 0.5deg resolution, 21 forecast members, Updates every 12 hours, forecast for 65 points spaced by 4 hours
         dictionary : dictionary, string, optional
             Dictionary that must be given when type is either
             'Forecast', 'Reanalysis' or 'Ensemble'.
             It specifies the dictionary to be used when reading netCDF
             and OPeNDAP files, allowing the correct retrieval of data.
             Acceptable values include 'ECMWF', 'NOAA' and 'UCAR' for
-            default dicitonaries which can generally be used to read
+            default dictionaries which can generally be used to read
             datasets from these institutes.
             Alternatively, a dictionary structure can also be given,
             specifying the short names used for time, latitude, longitude,
             pressure levels, temperature profile, geopotential or
             geopotential height profile, wind-u and wind-v profiles in
             the dataset given in the file parameter. Additionally,
             ensemble dictionaries must have the ensemble as well.
@@ -795,30 +795,30 @@
             profile. The float should be in units of Pa.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the pressure in Pa.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, pressure in Pa).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding pressure in Pa.
         temperature : float, string, array, callable, optional
             This defines the atmospheric temperature profile.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             than the the Standard Atmosphere temperature will be used.
             If a float is given, it will define a constant temperature
             profile. The float should be in units of K.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the temperature in K.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, temperature in K).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding temperature in K.
         wind_u : float, string, array, callable, optional
             This defines the atmospheric wind-u profile, corresponding
             the the magnitude of the wind speed heading East.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             it will be assumed to be constant and equal to 0.
@@ -826,15 +826,15 @@
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-u in m/s.
             If an array is given, it is expected to be an array of
             coordinates (height in meters, wind-u in m/s).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-u in m/s.
         wind_v : float, string, array, callable, optional
             This defines the atmospheric wind-v profile, corresponding
             the the magnitude of the wind speed heading North.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             it will be assumed to be constant and equal to 0.
@@ -842,15 +842,15 @@
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-v in m/s.
             If an array is given, it is expected to be an array of
             coordinates (height in meters, wind-v in m/s).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-v in m/s.
 
         Return
         ------
         None
         """
@@ -1154,16 +1154,16 @@
                         "v_wind": "vgrdprs",
                     }
                 # Process forecast or reanalysis
                 self.processEnsemble(file, dictionary)
             # Save dictionary and file
             self.atmosphericModelFile = file
             self.atmosphericModelDict = dictionary
-        elif type == "CostumAtmosphere":
-            self.processCostumAtmosphere(pressure, temperature, wind_u, wind_v)
+        elif type == "CustomAtmosphere":
+            self.processCustomAtmosphere(pressure, temperature, wind_u, wind_v)
         else:
             raise ValueError("Unknown model type.")
 
         # Calculate air density
         self.calculateDensityProfile()
 
         # Calculate speed of sound
@@ -1226,15 +1226,15 @@
         )
 
         # Set maximum expected height
         self.maxExpectedHeight = 80000
 
         return None
 
-    def processCostumAtmosphere(
+    def processCustomAtmosphere(
         self, pressure=None, temperature=None, wind_u=0, wind_v=0
     ):
         """Import pressure, temperature and wind profile given by user.
 
         Parameters
         ----------
         pressure : float, string, array, callable, optional
@@ -1245,30 +1245,30 @@
             profile. The float should be in units of Pa.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the pressure in Pa.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, pressure in Pa).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding pressure in Pa.
         temperature : float, string, array, callable, optional
             This defines the atmospheric temperature profile.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             than the the Standard Atmosphere temperature will be used.
             If a float is given, it will define a constant temperature
             profile. The float should be in units of K.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the temperature in K.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, temperature in K).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding temperature in K.
         wind_u : float, string, array, callable, optional
             This defines the atmospheric wind-u profile, corresponding
             the the magnitude of the wind speed heading East.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             it will be assumed constant and 0.
@@ -1276,15 +1276,15 @@
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-u in m/s.
             If an array is given, it is expected to be an array of
             coordinates (height in meters, wind-u in m/s).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-u in m/s.
         wind_v : float, string, array, callable, optional
             This defines the atmospheric wind-v profile, corresponding
             the the magnitude of the wind speed heading North.
             Should be given if the type parameter is 'CustomAtmosphere'. If not,
             it will be assumed constant and 0.
@@ -1292,15 +1292,15 @@
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-v in m/s.
             If an array is given, it is expected to be an array of
             coordinates (height in meters, wind-v in m/s).
-            Finally, a callable or function is also acepted. The
+            Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-v in m/s.
 
         Return
         ------
         None
         """
@@ -1308,22 +1308,22 @@
         maxExpectedHeight = 1000
 
         # Save pressure profile
         if pressure is None:
             # Use standard atmosphere
             self.pressure = self.pressureISA
         else:
-            # Use costum input
+            # Use custom input
             self.pressure = Function(
                 pressure,
                 inputs="Height Above Sea Level (m)",
                 outputs="Pressure (Pa)",
                 interpolation="linear",
             )
-            # Check maximum height of costum pressure input
+            # Check maximum height of custom pressure input
             if not callable(self.pressure.source):
                 maxExpectedHeight = max(self.pressure[-1, 0], maxExpectedHeight)
 
         # Save temperature profile
         if temperature is None:
             # Use standard atmosphere
             self.temperature = self.temperatureISA
@@ -1398,15 +1398,15 @@
         Upper Air Soundings database given by the url in file. Sets
         pressure, temperature, wind-u, wind-v profiles and surface elevation.
 
         Parameters
         ----------
         file : string
             URL of an upper air sounding data output from Wyoming
-            Upper Air Soundigs database.
+            Upper Air Soundings database.
             Example:
             http://weather.uwyo.edu/cgi-bin/sounding?region=samer&TYPE=TEXT%3ALIST&YEAR=2019&MONTH=02&FROM=0200&TO=0200&STNM=82599
             More can be found at:
             http://weather.uwyo.edu/upperair/sounding.html.
 
         Returns
         -------
@@ -1716,15 +1716,15 @@
         dictionary : dictionary
             Specifies the dictionary to be used when reading netCDF and
             OPeNDAP files, allowing for the correct retrieval of data.
             The dictionary structure should specify the short names
             used for time, latitude, longitude, pressure levels,
             temperature profile, geopotential or geopotential height
             profile, wind-u and wind-v profiles in the dataset given in
-            the file parameter. An example is the following dicitonary,
+            the file parameter. An example is the following dictionary,
             generally used to read OPeNDAP files from NOAA's NOMAD
             server:               {'time': 'time',
                                'latitude': 'lat',
                               'longitude': 'lon',
                                   'level': 'lev',
                             'temperature': 'tmpprs',
             'surface_geopotential_height': 'hgtsfc',
@@ -1745,16 +1745,16 @@
                 "Alternatively, use the Environment.setDate"
                 " method."
             )
         if self.lat is None:
             raise TypeError(
                 "Please specify Location (lat, lon). when "
                 "initializing this Environment. "
-                "Alternatively, use the Environment.setLoc"
-                "ation method."
+                "Alternatively, use the Environment."
+                "setLocation method."
             )
 
         # Read weather file
         weatherData = netCDF4.Dataset(file)
 
         # Get time, latitude and longitude data from file
         timeArray = weatherData.variables[dictionary["time"]]
@@ -2104,22 +2104,22 @@
         see Environment.selectEnsembleMemberMember().
 
         Parameters
         ----------
         file : string
             String containing path to local netCDF file or URL of an
             OPeNDAP file, such as NOAA's NOMAD or UCAR TRHEDDS server.
-        dicitonary : dictionary
+        dictionary : dictionary
             Specifies the dictionary to be used when reading netCDF and
             OPeNDAP files, allowing for the correct retrieval of data.
             The dictionary structure should specify the short names
             used for time, latitude, longitude, pressure levels,
             temperature profile, geopotential or geopotential height
             profile, wind-u and wind-v profiles in the dataset given in
-            the file parameter. An example is the following dicitonary,
+            the file parameter. An example is the following dictionary,
             generally used to read OPeNDAP files from NOAA's NOMAD
             server:               {'time': 'time',
                                'latitude': 'lat',
                               'longitude': 'lon',
                                   'level': 'lev',
                                'ensemble': 'ens',
             'surface_geopotential_height': 'hgtsfc',
@@ -2140,16 +2140,16 @@
                 "Alternatively, use the Environment.setDate"
                 " method."
             )
         if self.lat is None:
             raise TypeError(
                 "Please specify Location (lat, lon). when "
                 "initializing this Environment. "
-                "Alternatively, use the Environment.setLoc"
-                "ation method."
+                "Alternatively, use the Environment."
+                "setLocation method."
             )
 
         # Read weather file
         weatherData = netCDF4.Dataset(file)
 
         # Get time, latitude and longitude data from file
         timeArray = weatherData.variables[dictionary["time"]]
@@ -2669,15 +2669,15 @@
             outputs="Pressure (Pa)",
         )
 
         return None
 
     def calculateDensityProfile(self):
         """Compute the density of the atmosphere as a function of
-        heigth by using the formula rho = P/(RT). This function is
+        height by using the formula rho = P/(RT). This function is
         automatically called whenever a new atmospheric model is set.
 
         Parameters
         ----------
         None
 
         Returns
@@ -2698,15 +2698,15 @@
         # Save calculated density
         self.density = D
 
         return None
 
     def calculateSpeedOfSoundProfile(self):
         """Compute the speed of sound in the atmosphere as a function
-        of heigth by using the formula a = sqrt(gamma*R*T). This
+        of height by using the formula a = sqrt(gamma*R*T). This
         function is automatically called whenever a new atmospheric
         model is set.
 
         Parameters
         ----------
         None
 
@@ -3276,15 +3276,15 @@
         L = (5 - t + 9 * c + 4 * c * c) * ag * ag * ag * ag / 24
         M = (61 - 58 * t + t * t + 600 * c - 330 * e2lin) * (ag ** 6) / 720
 
         # Evaluate the final coordinates
         x = 500000 + K0 * n * (ag + J + K)
         y = N0 + K0 * (m + n * np.tan(lat) * (ag * ag / 2 + L + M))
 
-        # Convert the output lat and lon to degress
+        # Convert the output lat and lon to degrees
         lat = lat * 180 / np.pi
         lon = lon * 180 / np.pi
         lon_mc = lon_mc * 180 / np.pi
 
         # Calculate the UTM zone number
         utmZone = int((lon_mc + 183) / 6)
 
@@ -3324,15 +3324,15 @@
             latitude of the analysed point
         """
 
         if hemis == "N":
             y = y + 10000000
 
         # Calculate the Central Meridian from the UTM zone number
-        centralMeridian = utmZone * 6 - 183  # degress
+        centralMeridian = utmZone * 6 - 183  # degrees
 
         # Select the desired datum
         if datum == "SAD69":
             semiMajorAxis = 6378160.0
             flattening = 1 / 298.25
         elif datum == "WGS84":
             semiMajorAxis = 6378137.0
@@ -3471,15 +3471,15 @@
         Returns
         -------
         deg: float
             The degrees.
         min: float
             The arc minutes. 1 arc-minute = (1/60)*degree
         sec: float
-            The arc Seconds. 1 arc-secon = (1/360)*degree
+            The arc Seconds. 1 arc-second = (1/360)*degree
         """
 
         if angle < 0:
             signal = -1
         else:
             signal = 1
 
@@ -3490,15 +3490,15 @@
         #    angle, signal*deg, min, sec
         # ))
 
         return deg, min, sec
 
     def printEarthDetails(self):
         """[UNDER CONSTRUCTION]
-        Function to print informations about the Earth Model used in the
+        Function to print information about the Earth Model used in the
         Environment Class
 
         """
         # Print launch site details
         # print("Launch Site Details")
         # print("Launch Site Latitude: {:.5f}°".format(self.lat))
         # print("Launch Site Longitude: {:.5f}°".format(self.lon))
```

### Comparing `rocketpy-0.9.8/rocketpy/Flight.py` & `rocketpy-0.9.9/rocketpy/Flight.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         Flight.apogeeX : int, float
             X coordinate (positive east) of the center of mass of the
             rocket when it reaches apogee.
         Flight.apogeeY : int, float
             Y coordinate (positive north) of the center of mass of the
             rocket when it reaches apogee.
         Flight.apogee : int, float
-            Z coordinate, or altitute, of the center of mass of the
+            Z coordinate, or altitude, of the center of mass of the
             rocket when it reaches apogee.
         Flight.xImpact : int, float
             X coordinate (positive east) of the center of mass of the
             rocket when it impacts ground.
         Flight.yImpact : int, float
             Y coordinate (positive east) of the center of mass of the
             rocket when it impacts ground.
@@ -271,35 +271,35 @@
             magnitude relative to ground.
         Flight.pathAngle : Function
             Rocket's flight path angle, or the angle that the
             rocket's velocity makes with the horizontal (North-East)
             plane. Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
         Flight.attitudeVectorX : Function
-            Rocket's attiude vector, or the vector that points
+            Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the X
             direction (East) as a function of time.
             Can be called or accessed as array.
         Flight.attitudeVectorY : Function
-            Rocket's attiude vector, or the vector that points
+            Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the Y
             direction (East) as a function of time.
             Can be called or accessed as array.
         Flight.attitudeVectorZ : Function
-            Rocket's attiude vector, or the vector that points
+            Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the Z
             direction (East) as a function of time.
             Can be called or accessed as array.
         Flight.attitudeAngle : Function
-            Rocket's attiude angle, or the angle that the
+            Rocket's attitude angle, or the angle that the
             rocket's axis of symmetry makes with the horizontal (North-East)
             plane. Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
         Flight.lateralAttitudeAngle : Function
-            Rocket's lateral attiude angle, or the angle that the
+            Rocket's lateral attitude angle, or the angle that the
             rocket's axis of symmetry makes with plane defined by
             the launch rail direction and the Z (up) axis.
             Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
         Flight.phi : Function
             Rocket's Spin Euler Angle, φ, according to the 3-2-3 rotation
             system (NASA Standard Aerospace). Measured in degrees and
@@ -333,31 +333,31 @@
             as a function of time. Units in N. Usually just drag.
             Expressed as a function of time. Can be called or accessed
             as array.
             Direction 3 is in the rocket's body axis and points in the
             direction of cylindrical symmetry.
         Flight.M1 : Function
             Resultant moment (torque) perpendicular to rockets axis due to
-            aerodynamic forces and excentricity as a function of time.
+            aerodynamic forces and eccentricity as a function of time.
             Units in N*m.
             Expressed as a function of time. Can be called or accessed
             as array.
             Direction 1 is in the rocket's body axis and points perpendicular
             to the rocket's axis of cylindrical symmetry.
         Flight.M2 : Function
             Resultant moment (torque) perpendicular to rockets axis due to
-            aerodynamic forces and excentricity as a function of time.
+            aerodynamic forces and eccentricity as a function of time.
             Units in N*m.
             Expressed as a function of time. Can be called or accessed
             as array.
             Direction 2 is in the rocket's body axis and points perpendicular
             to the rocket's axis of cylindrical symmetry and direction 1.
         Flight.M3 : Function
             Resultant moment (torque) in rockets axis due to aerodynamic
-            forces and excentricity as a function of time. Units in N*m.
+            forces and eccentricity as a function of time. Units in N*m.
             Expressed as a function of time. Can be called or accessed
             as array.
             Direction 3 is in the rocket's body axis and points in the
             direction of cylindrical symmetry.
         Flight.aerodynamicLift : Function
             Resultant force perpendicular to rockets axis due to
             aerodynamic effects as a function of time. Units in N.
@@ -458,15 +458,15 @@
         Flight.freestreamSpeed : Function
             Freestream velocity magnitude, in m/s, as a function of time.
             Can be called or accessed as array.
         Flight.apogeeFreestreamSpeed : float
             Freestream speed of the rocket at apogee in m/s.
         Flight.MachNumber : Function
             Rocket's Mach number defined as its freestream speed
-            devided by the speed of sound at its altitude. Expressed
+            divided by the speed of sound at its altitude. Expressed
             as a function of time. Can be called or accessed as array.
         Flight.maxMachNumber : float
             Rocket's maximum Mach number experienced during flight.
         Flight.maxMachNumberTime : float
             Time at which the rocket experiences the maximum Mach number.
         Flight.ReynoldsNumber : Function
             Rocket's Reynolds number, using its diameter as reference
@@ -545,15 +545,15 @@
                                 xInit, yInit, zInit,
                                 vxInit, vyInit, vzInit,
                                 e0Init, e1Init, e2Init, e3Init,
                                 w1Init, w2Init, w3Init].
             If None, the initial solution will start with all null values,
             except for the euler parameters which will be calculated based
             on given values of inclination and heading. Default is None.
-        terminateOnApogee : boolean, optioanal
+        terminateOnApogee : boolean, optional
             Whether to terminate simulation when rocket reaches apogee.
             Default is False.
         maxTime : int, float, optional
             Maximum time in which to simulate trajectory in seconds.
             Using this without setting a maxTimeStep may cause unexpected
             errors. Default is 600.
         maxTimeStep : int, float, optional
@@ -623,15 +623,15 @@
         self.apogee = 0
         self.xImpact = 0
         self.yImpact = 0
         self.impactVelocity = 0
         self.impactState = np.array([0])
         self.parachuteEvents = []
         self.postProcessed = False
-        # Intialize solver monitors
+        # Initialize solver monitors
         self.functionEvaluations = []
         self.functionEvaluationsPerTimeStep = []
         self.timeSteps = []
         # Initialize solution state
         self.solution = []
         if self.initialSolution is None:
             # Initialize time and state variables
@@ -1135,15 +1135,15 @@
         # Retrieve integration data
         x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
 
         # Retrieve important quantities
         # Mass
         M = self.rocket.totalMass.getValueOpt(t)
 
-        # Get freestrean speed
+        # Get freestream speed
         freestreamSpeed = (
             (self.env.windVelocityX.getValueOpt(z) - vx) ** 2
             + (self.env.windVelocityY.getValueOpt(z) - vy) ** 2
             + (vz) ** 2
         ) ** 0.5
         freestreamMach = freestreamSpeed / self.env.speedOfSound.getValueOpt(z)
         dragCoeff = self.rocket.powerOnDrag.getValueOpt(freestreamMach)
@@ -1212,31 +1212,31 @@
         """
 
         # Retrieve integration data
         x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
         # Determine lift force and moment
         R1, R2 = 0, 0
         M1, M2, M3 = 0, 0, 0
-        # Determine current behaviour
+        # Determine current behavior
         if t < self.rocket.motor.burnOutTime:
             # Motor burning
             # Retrieve important motor quantities
             # Inertias
             Tz = self.rocket.motor.inertiaZ.getValueOpt(t)
             Ti = self.rocket.motor.inertiaI.getValueOpt(t)
             TzDot = self.rocket.motor.inertiaZDot.getValueOpt(t)
             TiDot = self.rocket.motor.inertiaIDot.getValueOpt(t)
             # Mass
             MtDot = self.rocket.motor.massDot.getValueOpt(t)
             Mt = self.rocket.motor.mass.getValueOpt(t)
             # Thrust
             Thrust = self.rocket.motor.thrust.getValueOpt(t)
             # Off center moment
-            M1 += self.rocket.thrustExcentricityX * Thrust
-            M2 -= self.rocket.thrustExcentricityY * Thrust
+            M1 += self.rocket.thrustEccentricityX * Thrust
+            M2 -= self.rocket.thrustEccentricityY * Thrust
         else:
             # Motor stopped
             # Retrieve important motor quantities
             # Inertias
             Tz, Ti, TzDot, TiDot = 0, 0, 0, 0
             # Mass
             MtDot, Mt = 0, 0
@@ -1268,15 +1268,15 @@
         a33 = 1 - 2 * (e1 ** 2 + e2 ** 2)
         # Transformation matrix: (123) -> (XYZ)
         K = [[a11, a12, a13], [a21, a22, a23], [a31, a32, a33]]
         # Transformation matrix: (XYZ) -> (123) or K transpose
         Kt = [[a11, a21, a31], [a12, a22, a32], [a13, a23, a33]]
 
         # Calculate Forces and Moments
-        # Get freestrean speed
+        # Get freestream speed
         windVelocityX = self.env.windVelocityX.getValueOpt(z)
         windVelocityY = self.env.windVelocityY.getValueOpt(z)
         freestreamSpeed = (
             (windVelocityX - vx) ** 2 + (windVelocityY - vy) ** 2 + (vz) ** 2
         ) ** 0.5
         freestreamMach = freestreamSpeed / self.env.speedOfSound.getValueOpt(z)
 
@@ -1285,16 +1285,16 @@
         if t > self.rocket.motor.burnOutTime:
             dragCoeff = self.rocket.powerOnDrag.getValueOpt(freestreamMach)
         else:
             dragCoeff = self.rocket.powerOffDrag.getValueOpt(freestreamMach)
         rho = self.env.density.getValueOpt(z)
         R3 = -0.5 * rho * (freestreamSpeed ** 2) * self.rocket.area * (dragCoeff)
         # Off center moment
-        M1 += self.rocket.cpExcentricityY * R3
-        M2 -= self.rocket.cpExcentricityX * R3
+        M1 += self.rocket.cpEccentricityY * R3
+        M2 -= self.rocket.cpEccentricityX * R3
         # Get rocket velocity in body frame
         vxB = a11 * vx + a21 * vy + a31 * vz
         vyB = a12 * vx + a22 * vy + a32 * vz
         vzB = a13 * vx + a23 * vy + a33 * vz
         # Calculate lift and moment for each component of the rocket
         for aerodynamicSurface in self.rocket.aerodynamicSurfaces:
             compCp = aerodynamicSurface[0][2]
@@ -1335,14 +1335,21 @@
                     compLiftYB = compLift * (compStreamVyB / liftDirNorm)
                     # Add to total lift force
                     R1 += compLiftXB
                     R2 += compLiftYB
                     # Add to total moment
                     M1 -= (compCp + a) * compLiftYB
                     M2 += (compCp + a) * compLiftXB
+            # Calculates Roll Moment
+            if aerodynamicSurface[-1] == "Fins":
+                Clfdelta, Cldomega, cantAngleRad = aerodynamicSurface[2]
+                if cantAngleRad != 0:
+                    Clf = Clfdelta * cantAngleRad
+                    Cld = Cldomega * omega3 / freestreamSpeed
+                    M3 += Clf - Cld
         # Calculate derivatives
         # Angular acceleration
         alpha1 = (
             M1
             - (
                 omega2 * omega3 * (Rz + Tz - Ri - Ti - mu * b ** 2)
                 + omega1
@@ -1412,15 +1419,15 @@
             self.pressure.append([t, self.env.pressure(z)])
             self.speedOfSound.append([t, self.env.speedOfSound(z)])
 
         return uDot
 
     def uDotParachute(self, t, u, postProcessing=False):
         """Calculates derivative of u state vector with respect to time
-        when rocket is flying under parachute. A 3 DOF aproximation is
+        when rocket is flying under parachute. A 3 DOF approximation is
         used.
 
         Parameters
         ----------
         t : float
             Time in seconds
         u : list
@@ -1489,15 +1496,15 @@
             self.speedOfSound.append([t, self.env.speedOfSound(z)])
 
         return [vx, vy, vz, ax, ay, az, 0, 0, 0, 0, 0, 0, 0]
 
     def postProcess(self):
         """Post-process all Flight information produced during
         simulation. Includes the calculation of maximum values,
-        calculation of secundary values such as energy and conversion
+        calculation of secondary values such as energy and conversion
         of lists to Function objects to facilitate plotting.
 
         Parameters
         ----------
         None
 
         Return
@@ -1547,25 +1554,25 @@
             sol[:, [0, 13]], "Time (s)", "ω3 (rad/s)", "spline", extrapolation="natural"
         )
 
         # Process second type of outputs - accelerations
         # Initialize acceleration arrays
         self.ax, self.ay, self.az = [], [], []
         self.alpha1, self.alpha2, self.alpha3 = [], [], []
-        # Go throught each time step and calculate accelerations
+        # Go through each time step and calculate accelerations
         # Get flight phases
         for phase_index, phase in self.timeIterator(self.flightPhases):
             initTime = phase.t
             finalTime = self.flightPhases[phase_index + 1].t
             currentDerivative = phase.derivative
             # Call callback functions
             for callback in phase.callbacks:
                 callback(self)
             # Loop through time steps in flight phase
-            for step in self.solution:  # Can be optmized
+            for step in self.solution:  # Can be optimized
                 if initTime < step[0] <= finalTime:
                     # Get derivatives
                     uDot = currentDerivative(step[0], step[1:])
                     # Get accelerations
                     ax, ay, az = uDot[3:6]
                     alpha1, alpha2, alpha3 = uDot[10:]
                     # Save accelerations
@@ -1589,25 +1596,25 @@
         self.pressure, self.density, self.dynamicViscosity, self.speedOfSound = (
             [],
             [],
             [],
             [],
         )
         self.windVelocityX, self.windVelocityY = [], []
-        # Go throught each time step and calculate forces and atmospheric values
+        # Go through each time step and calculate forces and atmospheric values
         # Get flight phases
         for phase_index, phase in self.timeIterator(self.flightPhases):
             initTime = phase.t
             finalTime = self.flightPhases[phase_index + 1].t
             currentDerivative = phase.derivative
             # Call callback functions
             for callback in phase.callbacks:
                 callback(self)
             # Loop through time steps in flight phase
-            for step in self.solution:  # Can be optmized
+            for step in self.solution:  # Can be optimized
                 if initTime < step[0] <= finalTime or (initTime == 0 and step[0] == 0):
                     # Call derivatives in post processing mode
                     uDot = currentDerivative(step[0], step[1:], postProcessing=True)
         # Convert forces and atmospheric arrays to functions
         self.R1 = Function(self.R1, "Time (s)", "R1 (N)", "spline")
         self.R2 = Function(self.R2, "Time (s)", "R2 (N)", "spline")
         self.R3 = Function(self.R3, "Time (s)", "R3 (N)", "spline")
@@ -1669,24 +1676,24 @@
         lateralVectorY = np.cos(lateralVectorAngle)
         attitudeLateralProj = (
             lateralVectorX * self.attitudeVectorX[:, 1]
             + lateralVectorY * self.attitudeVectorY[:, 1]
         )
         attitudeLateralProjX = attitudeLateralProj * lateralVectorX
         attitudeLateralProjY = attitudeLateralProj * lateralVectorY
-        attiutdeLateralPlaneProjX = self.attitudeVectorX[:, 1] - attitudeLateralProjX
-        attiutdeLateralPlaneProjY = self.attitudeVectorY[:, 1] - attitudeLateralProjY
-        attiutdeLateralPlaneProjZ = self.attitudeVectorZ[:, 1]
-        attiutdeLateralPlaneProj = (
-            attiutdeLateralPlaneProjX ** 2
-            + attiutdeLateralPlaneProjY ** 2
-            + attiutdeLateralPlaneProjZ ** 2
+        attitudeLateralPlaneProjX = self.attitudeVectorX[:, 1] - attitudeLateralProjX
+        attitudeLateralPlaneProjY = self.attitudeVectorY[:, 1] - attitudeLateralProjY
+        attitudeLateralPlaneProjZ = self.attitudeVectorZ[:, 1]
+        attitudeLateralPlaneProj = (
+            attitudeLateralPlaneProjX ** 2
+            + attitudeLateralPlaneProjY ** 2
+            + attitudeLateralPlaneProjZ ** 2
         ) ** 0.5
         lateralAttitudeAngle = (180 / np.pi) * np.arctan2(
-            attitudeLateralProj, attiutdeLateralPlaneProj
+            attitudeLateralProj, attitudeLateralPlaneProj
         )
         lateralAttitudeAngle = np.column_stack(
             [self.attitudeVectorZ[:, 0], lateralAttitudeAngle]
         )
         self.lateralAttitudeAngle = Function(
             lateralAttitudeAngle, "Time (s)", "Lateral Attitude Angle (°)"
         )
@@ -2014,17 +2021,17 @@
         None
         """
         # Post-process results
         if self.postProcessed is False:
             self.postProcess()
 
         # Get index of out of rail time
-        outOfRailTimeIndexs = np.nonzero(self.x[:, 0] == self.outOfRailTime)
+        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
         outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexs) == 0 else outOfRailTimeIndexs[0][0]
+            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
         )
 
         # Get index of time before parachute event
         if len(self.parachuteEvents) > 0:
             eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
             eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
         else:
@@ -2285,24 +2292,24 @@
         Return
         ------
         None
         """
         vF = self.outOfRailVelocity
 
         # Convert angle to radians
-        tetha = self.inclination * np.pi / 180
+        theta = self.inclination * np.pi / 180
         stallAngle = stallAngle * np.pi / 180
 
-        c = (math.cos(stallAngle) ** 2 - math.cos(tetha) ** 2) / math.sin(
+        c = (math.cos(stallAngle) ** 2 - math.cos(theta) ** 2) / math.sin(
             stallAngle
         ) ** 2
         wV = (
-            2 * vF * math.cos(tetha) / c
+            2 * vF * math.cos(theta) / c
             + (
-                4 * vF * vF * math.cos(tetha) * math.cos(tetha) / (c ** 2)
+                4 * vF * vF * math.cos(theta) * math.cos(theta) / (c ** 2)
                 + 4 * 1 * vF * vF / c
             )
             ** 0.5
         ) / 2
 
         # Convert stallAngle to degrees
         stallAngle = stallAngle * 180 / np.pi
@@ -2669,17 +2676,17 @@
         None
         """
         # Post-process results
         if self.postProcessed is False:
             self.postProcess()
 
         # Get index of out of rail time
-        outOfRailTimeIndexs = np.nonzero(self.x[:, 0] == self.outOfRailTime)
+        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
         outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexs) == 0 else outOfRailTimeIndexs[0][0]
+            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
         )
 
         # Get index of time before parachute event
         if len(self.parachuteEvents) > 0:
             eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
             eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
         else:
@@ -2796,17 +2803,17 @@
         None
         """
         # Post-process results
         if self.postProcessed is False:
             self.postProcess()
 
         # Get index of out of rail time
-        outOfRailTimeIndexs = np.nonzero(self.x[:, 0] == self.outOfRailTime)
+        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
         outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexs) == 0 else outOfRailTimeIndexs[0][0]
+            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
         )
 
         # Get index of time before parachute event
         if len(self.parachuteEvents) > 0:
             eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
             eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
         else:
@@ -2894,17 +2901,17 @@
         None
         """
         # Post-process results
         if self.postProcessed is False:
             self.postProcess()
 
         # Get index of out of rail time
-        outOfRailTimeIndexs = np.nonzero(self.x[:, 0] == self.outOfRailTime)
+        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
         outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexs) == 0 else outOfRailTimeIndexs[0][0]
+            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
         )
 
         # Trajectory Fluid Mechanics Plots
         fig10 = plt.figure(figsize=(9, 12))
 
         ax1 = plt.subplot(411)
         ax1.plot(self.MachNumber[:, 0], self.MachNumber[:, 1])
@@ -2955,15 +2962,15 @@
         plt.subplots_adjust(hspace=0.5)
         plt.show()
 
         return None
 
     def calculateFinFlutterAnalysis(self, finThickness, shearModulus):
         """Calculate, create and plot the Fin Flutter velocity, based on the
-        pressure profile provided by Atmosferic model selected. It considers the
+        pressure profile provided by Atmospheric model selected. It considers the
         Flutter Boundary Equation that is based on a calculation published in
         NACA Technical Paper 4197.
         Be careful, these results are only estimates of a real problem and may
         not be useful for fins made from non-isotropic materials. These results
         should not be used as a way to fully prove the safety of any rocket’s fins.
         IMPORTANT: This function works if only a single set of fins is added
 
@@ -3181,15 +3188,15 @@
 
         return None
 
     def plotPressureSignals(self):
         """Prints out all Parachute Trigger Pressure Signals.
         This function can be called also for plot pressure data for flights
         without Parachutes, in this case the Pressure Signals will be simply
-        the pressure provided by the atmosfericModel, at Flight z positions.
+        the pressure provided by the atmosphericModel, at Flight z positions.
         This means that no noise will be considered if at least one parachute
         has not been added.
 
         This function aims to help the engineer to visually check if there
         are anomalies with the Flight Simulation.
 
         Parameters
@@ -3232,15 +3239,15 @@
         although it is not possible to get a noisy pressure signal if no
         parachute is added.
 
         If a parachute is added, the file will contain 3 columns: time in seconds,
         clean pressure in Pascals and noisy pressure in Pascals. For flights without
         parachutes, the third column will be discarded
 
-        This function was created especially for the Projeto Jupiter Eletronics
+        This function was created especially for the Projeto Jupiter Electronics
         Subsystems team and aims to help in configuring microcontrollers.
 
         Parameters
         ----------
         fileName : string
             The final file name,
         timeStep : float
@@ -3365,19 +3372,19 @@
             W.remove()
             S.remove()
             # Calculate rocket position
             Rx, Ry, Rz = self.x(t), self.y(t), self.z(t)
             Ru = 1 * (2 * (self.e1(t) * self.e3(t) + self.e0(t) * self.e2(t)))
             Rv = 1 * (2 * (self.e2(t) * self.e3(t) - self.e0(t) * self.e1(t)))
             Rw = 1 * (1 - 2 * (self.e1(t) ** 2 + self.e2(t) ** 2))
-            # Caclulate rocket Mach number
+            # Calculate rocket Mach number
             Vx = self.vx(t) / 340.40
             Vy = self.vy(t) / 340.40
             Vz = self.vz(t) / 340.40
-            # Caculate wind Mach Number
+            # Calculate wind Mach Number
             z = self.z(t)
             Wx = self.env.windVelocityX(z) / 20
             Wy = self.env.windVelocityY(z) / 20
             # Calculate freestream Mach Number
             Sx = self.streamVelocityX(t) / 340.40
             Sy = self.streamVelocityY(t) / 340.40
             Sz = self.streamVelocityZ(t) / 340.40
```

### Comparing `rocketpy-0.9.8/rocketpy/Function.py` & `rocketpy-0.9.9/rocketpy/Function.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             self.__extrapolation__ = None
         # Handle ndarray source
         else:
             # Check to see if dimensions match incoming data set
             newTotalDim = len(source[0, :])
             oldTotalDim = self.__domDim__ + self.__imgDim__
             dV = self.__inputs__ == ["Scalar"] and self.__outputs__ == ["Scalar"]
-            # If they dont, update default values or throw error
+            # If they don't, update default values or throw error
             if newTotalDim != oldTotalDim:
                 if dV:
                     # Update dimensions and inputs
                     self.__domDim__ = newTotalDim - 1
                     self.__inputs__ = self.__domDim__ * self.__inputs__
                 else:
                     # User has made a mistake inputting inputs and outputs
@@ -287,15 +287,15 @@
             extrapolation = 1  # Extrapolation is natural
         else:
             extrapolation = 2  # Extrapolation is constant
 
         # Crete method to interpolate this info for each interpolation type
         if self.__interpolation__ == "spline":
             coeffs = self.__splineCoefficients__
-            # @jit(nopython=True)
+
             def getValueOpt(x):
                 xInterval = np.searchsorted(xData, x)
                 # Interval found... interpolate... or extrapolate
                 if xmin <= x <= xmax:
                     # Interpolate
                     xInterval = xInterval if xInterval != 0 else 1
                     a = coeffs[:, xInterval - 1]
@@ -312,15 +312,15 @@
                     else:  # Extrapolation is set to constant
                         y = yData[0] if x < xmin else yData[-1]
                 return y
 
             self.getValueOpt = getValueOpt
 
         elif self.__interpolation__ == "linear":
-            # @jit(nopython=True)
+
             def getValueOpt(x):
                 xInterval = np.searchsorted(xData, x)
                 # Interval found... interpolate... or extrapolate
                 if xmin <= x <= xmax:
                     # Interpolate
                     dx = float(xData[xInterval] - xData[xInterval - 1])
                     dy = float(yData[xInterval] - yData[xInterval - 1])
@@ -340,15 +340,15 @@
                         y = yData[0] if x < xmin else yData[-1]
                 return y
 
             self.getValueOpt = getValueOpt
 
         elif self.__interpolation__ == "akima":
             coeffs = np.array(self.__akimaCoefficients__)
-            # @jit(nopython=True)
+
             def getValueOpt(x):
                 xInterval = np.searchsorted(xData, x)
                 # Interval found... interpolate... or extrapolate
                 if xmin <= x <= xmax:
                     # Interpolate
                     xInterval = xInterval if xInterval != 0 else 1
                     a = coeffs[4 * xInterval - 4 : 4 * xInterval]
@@ -364,15 +364,15 @@
                         y = yData[0] if x < xmin else yData[-1]
                 return y
 
             self.getValueOpt = getValueOpt
 
         elif self.__interpolation__ == "polynomial":
             coeffs = self.__polynomialCoefficients__
-            # @jit(nopython=True)
+
             def getValueOpt(x):
                 # Interpolate... or extrapolate
                 if xmin <= x <= xmax:
                     # Interpolate
                     y = 0
                     for i in range(len(coeffs)):
                         y += coeffs[i] * (x ** i)
@@ -811,15 +811,15 @@
 
     def getValueOpt2(self, *args):
         """DEPRECATED!! - See Function.getValueOpt for new version.
         This method returns the value of the Function at the specified
         point in a limited but optimized manner. See Function.getValue for an
         implementation which allows more kinds of inputs.
         This method optimizes the Function.getValue method by only
-        implementing function evaluations of single inputes, i.e., it is not
+        implementing function evaluations of single inputs, i.e., it is not
         vectorized. Furthermore, it actually implements a different method
         for each interpolation type, eliminating some if statements.
         Finally, it uses Numba to compile the methods, which further optimizes
         the implementation.
         The code below is here for documentation purposes only. It is
         overwritten for all instances by the Function.setGetValuteOpt2 method.
 
@@ -1011,15 +1011,15 @@
         forceData=False,
         forcePoints=False,
         returnObject=False,
     ):
         """Plot 1-Dimensional Function, from a lower limit to an upper limit,
         by sampling the Function several times in the interval. The title of
         the graph is given by the name of the axes, which are taken from
-        the Function`s input and ouput names.
+        the Function`s input and output names.
 
         Parameters
         ----------
         lower : scalar, optional
             The lower limit of the interval in which the function is to be
             ploted. The default value for function type Functions is 0. By
             contrast, if the Function is given by a dataset, the default
```

### Comparing `rocketpy-0.9.8/rocketpy/Rocket.py` & `rocketpy-0.9.9/rocketpy/Rocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,25 +66,25 @@
             Function of time expressing the total mass of the rocket,
             defined as the sum of the propellant mass and the rocket
             mass without propellant.
         Rocket.thrustToWeight : Function
             Function of time expressing the motor thrust force divided by rocket
             weight. The gravitational acceleration is assumed as 9.80665 m/s^2.
 
-        Excentricity attributes:
-        Rocket.cpExcentricityX : float
+        Eccentricity attributes:
+        Rocket.cpEccentricityX : float
             Center of pressure position relative to center of mass in the x
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.cpExcentricityY : float
+        Rocket.cpEccentricityY : float
             Center of pressure position relative to center of mass in the y
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.thrustExcentricityY : float
+        Rocket.thrustEccentricityY : float
             Thrust vector position relative to center of mass in the y
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.thrustExcentricityX : float
+        Rocket.thrustEccentricityX : float
             Thrust vector position relative to center of mass in the x
             axis, perpendicular to axis of cylindrical symmetry, in meters.
 
         Parachute attributes:
         Rocket.parachutes : list
             List of parachutes of the rocket.
             Each parachute has the following attributes:
@@ -222,19 +222,19 @@
         self.radius = radius
         self.area = np.pi * self.radius ** 2
 
         # Center of mass distance to points of interest
         self.distanceRocketNozzle = distanceRocketNozzle
         self.distanceRocketPropellant = distanceRocketPropellant
 
-        # Excentricity data initialization
-        self.cpExcentricityX = 0
-        self.cpExcentricityY = 0
-        self.thrustExcentricityY = 0
-        self.thrustExcentricityX = 0
+        # Eccentricity data initialization
+        self.cpEccentricityX = 0
+        self.cpEccentricityY = 0
+        self.thrustEccentricityY = 0
+        self.thrustEccentricityX = 0
 
         # Parachute data initialization
         self.parachutes = []
 
         # Rail button data initialization
         self.railButtons = None
 
@@ -359,19 +359,19 @@
         Returns
         -------
         self.staticMargin : float
             Float value corresponding to rocket static margin when
             loaded with propellant in units of rocket diameter or
             calibers.
         """
-        # Initialize total lift coeficient derivative and center of pressure
+        # Initialize total lift coefficient derivative and center of pressure
         self.totalLiftCoeffDer = 0
         self.cpPosition = 0
 
-        # Calculate total lift coeficient derivative and center of pressure
+        # Calculate total lift coefficient derivative and center of pressure
         if len(self.aerodynamicSurfaces) > 0:
             for aerodynamicSurface in self.aerodynamicSurfaces:
                 self.totalLiftCoeffDer += aerodynamicSurface[1].differentiate(
                     x=1e-2, dx=1e-3
                 )
                 self.cpPosition += (
                     aerodynamicSurface[1].differentiate(x=1e-2, dx=1e-3)
@@ -432,15 +432,19 @@
             cpz = distanceToCM - (length / 3) * (1 + (1 - r) / (1 - r ** 2))
         else:
             cpz = distanceToCM + (length / 3) * (1 + (1 - r) / (1 - r ** 2))
 
         # Calculate clalpha
         clalpha = -2 * (1 - r ** (-2)) * (topRadius / rref) ** 2
         cldata = Function(
-            lambda x: clalpha * x, "Alpha (rad)", "Cl", interpolation="linear"
+            lambda x: clalpha * x,
+            "Alpha (rad)",
+            "Cl",
+            interpolation="linear",
+            extrapolation="natural",
         )
 
         # Store values as new aerodynamic surface
         tail = [(0, 0, cpz), cldata, "Tail"]
         self.aerodynamicSurfaces.append(tail)
 
         # Refresh static margin calculation
@@ -455,15 +459,15 @@
         along the rocket and its derivative of the coefficient of lift
         in respect to angle of attack.
 
 
         Parameters
         ----------
         length : int, float
-            Nose cone length or height in meters. Must be a postive
+            Nose cone length or height in meters. Must be a positive
             value.
         kind : string
             Nose cone type. Von Karman, conical, ogive, and lvhaack are
             supported.
         distanceToCM : int, float
             Nose cone position relative to rocket unloaded center of
             mass, considering positive direction from center of mass to
@@ -510,15 +514,23 @@
         # Refresh static margin calculation
         self.evaluateStaticMargin()
 
         # Return self
         return self.aerodynamicSurfaces[-1]
 
     def addFins(
-        self, n, span, rootChord, tipChord, distanceToCM, radius=0, airfoil=None
+        self,
+        n,
+        span,
+        rootChord,
+        tipChord,
+        distanceToCM,
+        radius=0,
+        cantAngle=0,
+        airfoil=None,
     ):
         """Create a fin set, storing its parameters as part of the
         aerodynamicSurfaces list. Its parameters are the axial position
         along the rocket and its derivative of the coefficient of lift
         in respect to angle of attack.
 
         Parameters
@@ -537,38 +549,49 @@
             nose cone. Consider the center point belonging to the top
             of the fins to calculate distance.
         radius : int, float, optional
             Reference radius to calculate lift coefficient. If 0, which
             is default, use rocket radius. Otherwise, enter the radius
             of the rocket in the section of the fins, as this impacts
             its lift coefficient.
+        cantAngle : int, float, optional
+            Fins cant angle with respect to the rocket centerline. Must
+            be given in degrees.
         airfoil : string
             Fin's lift curve. It must be a .csv file. The .csv file shall
             contain no headers and the first column must specify time in
             seconds, while the second column specifies lift coefficient. Lift
-            coeffitient is adimentional.
+            coefficient is dimensionaless.
 
         Returns
         -------
         cldata : Function
             Object of the Function class. Contains fin's lift data.
         self : Rocket
             Object of the Rocket class.
         """
 
         # Retrieve parameters for calculations
         Cr = rootChord
         Ct = tipChord
         Yr = rootChord + tipChord
         s = span
+        Af = Yr * s / 2  # fin area
+        Ymac = (
+            (s / 3) * (Cr + 2 * Ct) / Yr
+        )  # span wise position of fin's mean aerodynamic chord
         Lf = np.sqrt((rootChord / 2 - tipChord / 2) ** 2 + span ** 2)
         radius = self.radius if radius == 0 else radius
         d = 2 * radius
+        cantAngleRad = np.radians(cantAngle)
+        trapezoidalConstant = ((Yr) / 2) * (radius ** 2) * s
+        trapezoidalConstant += ((Cr + 2 * Ct) / 3) * radius * (s ** 2)
+        trapezoidalConstant += ((Cr + 3 * Ct) / 12) * (s ** 3)
 
-        # Save geometric parameters for later Fin Flutter Analysis
+        # Save geometric parameters for later Fin Flutter Analysis and Roll Moment Calculation
         self.rootChord = Cr
         self.tipChord = Ct
         self.span = s
         self.distanceRocketFins = distanceToCM
 
         # Calculate cp position relative to cm
         if distanceToCM < 0:
@@ -588,17 +611,25 @@
             clalpha = (4 * n * (s / d) ** 2) / (1 + np.sqrt(1 + (2 * Lf / Yr) ** 2))
             clalpha *= 1 + radius / (s + radius)
 
             # # Create a function of lift values by attack angle
             cldata = Function(
                 lambda x: clalpha * x, "Alpha (rad)", "Cl", interpolation="linear"
             )
+            # Parameters for Roll Moment. Documented at: https://github.com/Projeto-Jupiter/RocketPy/blob/develop/docs/technical/aerodynamics/Roll_Equations.pdf
+            clfDelta = n * (Ymac + radius) * clalpha / d
+            cldOmega = (
+                n * clalpha * np.cos(cantAngleRad) * trapezoidalConstant / (Af * d)
+            )
+            rollParameters = (
+                [clfDelta, cldOmega, cantAngleRad] if cantAngleRad != 0 else [0, 0, 0]
+            )
 
             # Store values
-            fin = [(0, 0, cpz), cldata, "Fins"]
+            fin = [(0, 0, cpz), cldata, rollParameters, "Fins"]
             self.aerodynamicSurfaces.append(fin)
 
             # Refresh static margin calculation
             self.evaluateStaticMargin()
 
             # Return self
             return self.aerodynamicSurfaces[-1]
@@ -635,29 +666,38 @@
                     / (2 + FD * (1 + (4 / FD ** 2)) ** 0.5)
                 )
                 return Cnalfa1
 
             # Import the lift curve as a function of lift values by attack angle
             read = genfromtxt(airfoil, delimiter=",")
 
-            # Aplies number of fins to lift coefficient data
+            # Applies number of fins to lift coefficient data
             data = [[cl[0], (n / 2) * cnalfa1(cl[1])] for cl in read]
             cldata = Function(
                 data,
                 "Alpha (rad)",
                 "Cl",
                 interpolation="linear",
                 extrapolation="natural",
             )
 
             # Takes an approximation to an angular coefficient
             clalpha = cldata.differentiate(x=0, dx=1e-2)
 
+            # Parameters for Roll Moment. Documented at: https://github.com/Projeto-Jupiter/RocketPy/blob/develop/docs/technical/aerodynamics/Roll_Equations.pdf
+            clfDelta = n * (Ymac + radius) * clalpha / d
+            cldOmega = (
+                n * clalpha * np.cos(cantAngleRad) * trapezoidalConstant / (Af * d)
+            )
+            rollParameters = (
+                [clfDelta, cldOmega, cantAngleRad] if cantAngleRad != 0 else [0, 0, 0]
+            )
+
             # Store values
-            fin = [(0, 0, cpz), cldata, "Fins"]
+            fin = [(0, 0, cpz), cldata, rollParameters, "Fins"]
             self.aerodynamicSurfaces.append(fin)
 
             # Refresh static margin calculation
             self.evaluateStaticMargin()
 
             # Return self
             return self.aerodynamicSurfaces[-1]
@@ -737,15 +777,15 @@
 
         # Return self
         return self.parachutes[-1]
 
     def setRailButtons(self, distanceToCM, angularPosition=45):
         """Adds rail buttons to the rocket, allowing for the
         calculation of forces exerted by them when the rocket is
-        slinding in the launch rail. Furthermore, rail buttons are
+        sliding in the launch rail. Furthermore, rail buttons are
         also needed for the simulation of the planar flight phase,
         when the rocket experiences 3 degrees of freedom motion while
         only one rail button is still in the launch rail.
 
         Parameters
         ----------
         distanceToCM : tuple, list, array
@@ -771,20 +811,20 @@
         if distanceToCM[0] < distanceToCM[1]:
             distanceToCM.reverse()
         # Save
         self.railButtons = self.railButtonPair(distanceToCM, angularPosition)
 
         return None
 
-    def addCMExcentricity(self, x, y):
+    def addCMEccentricity(self, x, y):
         """Moves line of action of aerodynamic and thrust forces by
-        equal translation ammount to simulate an excentricity in the
+        equal translation amount to simulate an eccentricity in the
         position of the center of mass of the rocket relative to its
         geometrical center line. Should not be used together with
-        addCPExentricity and addThrustExentricity.
+        addCPEccentricity and addThrustEccentricity.
 
         Parameters
         ----------
         x : float
             Distance in meters by which the CM is to be translated in
             the x direction relative to geometrical center line.
         y : float
@@ -793,27 +833,27 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move center of pressure to -x and -y
-        self.cpExcentricityX = -x
-        self.cpExcentricityY = -y
+        self.cpEccentricityX = -x
+        self.cpEccentricityY = -y
 
         # Move thrust center by -x and -y
-        self.thrustExcentricityY = -x
-        self.thrustExcentricityX = -y
+        self.thrustEccentricityY = -x
+        self.thrustEccentricityX = -y
 
         # Return self
         return self
 
-    def addCPExentricity(self, x, y):
+    def addCPEccentricity(self, x, y):
         """Moves line of action of aerodynamic forces to simulate an
-        excentricity in the position of the center of pressure relative
+        eccentricity in the position of the center of pressure relative
         to the center of mass of the rocket.
 
         Parameters
         ----------
         x : float
             Distance in meters by which the CP is to be translated in
             the x direction relative to the center of mass axial line.
@@ -823,21 +863,21 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move center of pressure by x and y
-        self.cpExcentricityX = x
-        self.cpExcentricityY = y
+        self.cpEccentricityX = x
+        self.cpEccentricityY = y
 
         # Return self
         return self
 
-    def addThrustExentricity(self, x, y):
+    def addThrustEccentricity(self, x, y):
         """Moves line of action of thrust forces to simulate a
         disalignment of the thrust vector and the center of mass.
 
         Parameters
         ----------
         x : float
             Distance in meters by which the line of action of the
@@ -850,16 +890,16 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move thrust line by x and y
-        self.thrustExcentricityY = x
-        self.thrustExcentricityX = y
+        self.thrustEccentricityY = x
+        self.thrustEccentricityX = y
 
         # Return self
         return self
 
     def info(self):
         """Prints out a summary of the data and graphs available about
         the Rocket.
@@ -936,15 +976,15 @@
             + " m"
         )
         print(
             "Rocket Center of Mass - Rocket Loaded Center of Mass: "
             + "{:.3f}".format(self.centerOfMass(0))
             + " m"
         )
-        print("\nAerodynamic Coponents Parameters")
+        print("\nAerodynamic Components Parameters")
         print("Currently not implemented.")
 
         # Print rocket aerodynamics quantities
         print("\nAerodynamics Lift Coefficient Derivatives")
         for aerodynamicSurface in self.aerodynamicSurfaces:
             name = aerodynamicSurface[-1]
             clalpha = aerodynamicSurface[1].differentiate(x=1e-2, dx=1e-3)
```

### Comparing `rocketpy-0.9.8/rocketpy/SolidMotor.py` & `rocketpy-0.9.9/rocketpy/SolidMotor.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,46 +224,44 @@
         self.grainNumber = grainNumber
         self.grainSeparation = grainSeparation
         self.grainDensity = grainDensity
         self.grainOuterRadius = grainOuterRadius
         self.grainInitialInnerRadius = grainInitialInnerRadius
         self.grainInitialHeight = grainInitialHeight
         # Other quantities that will be computed
-        self.exhaustVelocity = None
         self.massDot = None
         self.mass = None
         self.grainInnerRadius = None
         self.grainHeight = None
         self.burnArea = None
         self.Kn = None
         self.burnRate = None
         self.inertiaI = None
         self.inertiaIDot = None
         self.inertiaZ = None
-        self.inertiaDot = None
+        self.inertiaZDot = None
         self.maxThrust = None
         self.maxThrustTime = None
         self.averageThrust = None
 
-        # Compute uncalculated quantities
+        # Compute quantities
         # Thrust information - maximum and average
         self.maxThrust = np.amax(self.thrust.source[:, 1])
         maxThrustIndex = np.argmax(self.thrust.source[:, 1])
         self.maxThrustTime = self.thrust.source[maxThrustIndex, 0]
         self.averageThrust = self.totalImpulse / self.burnOutTime
         # Grains initial geometrical parameters
         self.grainInitialVolume = (
             self.grainInitialHeight
             * np.pi
             * (self.grainOuterRadius ** 2 - self.grainInitialInnerRadius ** 2)
         )
         self.grainInitialMass = self.grainDensity * self.grainInitialVolume
         self.propellantInitialMass = self.grainNumber * self.grainInitialMass
         # Dynamic quantities
-        self.evaluateExhaustVelocity()
         self.evaluateMassDot()
         self.evaluateMass()
         self.evaluateGeometry()
         self.evaluateInertia()
 
     def reshapeThrustCurve(
         self, burnTime, totalImpulse, oldTotalImpulse=None, startAtZero=True
@@ -293,15 +291,14 @@
         Returns
         -------
         None
         """
         # Retrieve current thrust curve data points
         timeArray = self.thrust.source[:, 0]
         thrustArray = self.thrust.source[:, 1]
-
         # Move start to time = 0
         if startAtZero and timeArray[0] != 0:
             timeArray = timeArray - timeArray[0]
 
         # Reshape time - set burn time to burnTime
         self.thrust.source[:, 0] = (burnTime / timeArray[-1]) * timeArray
         self.burnOutTime = burnTime
@@ -335,38 +332,31 @@
         """
         # Calculate total impulse
         self.totalImpulse = self.thrust.integral(0, self.burnOutTime)
 
         # Return total impulse
         return self.totalImpulse
 
-    def evaluateExhaustVelocity(self):
+    @property
+    def exhaustVelocity(self):
         """Calculates and returns exhaust velocity by assuming it
         as a constant. The formula used is total impulse/propellant
         initial mass. The value is also stored in
         self.exhaustVelocity.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         self.exhaustVelocity : float
             Constant gas exhaust velocity of the motor.
         """
-        # Calculate total impulse if not yet done so
-        if self.totalImpulse is None:
-            self.evaluateTotalImpulse()
-
-        # Calculate exhaust velocity
-        self.exhaustVelocity = self.totalImpulse / self.propellantInitialMass
-
-        # Return exhaust velocity
-        return self.exhaustVelocity
+        return self.totalImpulse / self.propellantInitialMass
 
     def evaluateMassDot(self):
         """Calculates and returns the time derivative of propellant
         mass by assuming constant exhaust velocity. The formula used
         is the opposite of thrust divided by exhaust velocity. The
         result is a function of time, object of the Function class,
         which is stored in self.massDot.
@@ -377,18 +367,14 @@
 
         Returns
         -------
         self.massDot : Function
             Time derivative of total propellant mas as a function
             of time.
         """
-        # Calculate exhaust velocity if not done so already
-        if self.exhaustVelocity is None:
-            self.evaluateExhaustVelocity()
-
         # Create mass dot Function
         self.massDot = self.thrust / (-self.exhaustVelocity)
         self.massDot.setOutputs("Mass Dot (kg/s)")
         self.massDot.setExtrapolation("zero")
 
         # Return Function
         return self.massDot
@@ -431,14 +417,18 @@
             self.interpolate,
             "constant",
         )
 
         # Return Mass Function
         return self.mass
 
+    @property
+    def throatArea(self):
+        return np.pi * self.throatRadius ** 2
+
     def evaluateGeometry(self):
         """Calculates grain inner radius and grain height as a
         function of time by assuming that every propellant mass
         burnt is exhausted. In order to do that, a system of
         differential equations is solved using scipy.integrate.
         odeint. Furthermore, the function calculates burn area,
         burn rate and Kn as a function of time using the previous
@@ -460,18 +450,18 @@
         """
         # Define initial conditions for integration
         y0 = [self.grainInitialInnerRadius, self.grainInitialHeight]
 
         # Define time mesh
         t = self.massDot.source[:, 0]
 
-        # Define system of differential equations
         density = self.grainDensity
         rO = self.grainOuterRadius
 
+        # Define system of differential equations
         def geometryDot(y, t):
             grainMassDot = self.massDot(t) / self.grainNumber
             rI, h = y
             rIDot = (
                 -0.5 * grainMassDot / (density * np.pi * (rO ** 2 - rI ** 2 + rI * h))
             )
             hDot = 1.0 * grainMassDot / (density * np.pi * (rO ** 2 - rI ** 2 + rI * h))
@@ -493,48 +483,82 @@
             "Time (s)",
             "Grain Height (m)",
             self.interpolate,
             "constant",
         )
 
         # Create functions describing burn rate, Kn and burn area
-        # Burn Area
+        self.evaluateBurnArea()
+        self.evaluateKn()
+        self.evaluateBurnRate()
+
+        return [self.grainInnerRadius, self.grainHeight]
+
+    def evaluateBurnArea(self):
+        """Calculates the BurnArea of the grain for
+        each time. Assuming that the grains are cylindrical
+        BATES grains.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        burnArea : Function
+        Function representing the burn area progression with the time.
+        """
         self.burnArea = (
             2
             * np.pi
             * (
                 self.grainOuterRadius ** 2
                 - self.grainInnerRadius ** 2
                 + self.grainInnerRadius * self.grainHeight
             )
             * self.grainNumber
         )
         self.burnArea.setOutputs("Burn Area (m2)")
-        # Kn
-        throatArea = np.pi * (self.throatRadius) ** 2
+        return self.burnArea
+
+    def evaluateBurnRate(self):
+        """Calculates the BurnRate with respect to time.
+        This evaluation assumes that it was already
+        calculated the massDot, burnArea timeseries.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        burnRate : Function
+        Rate of progression of the inner radius during the combustion.
+        """
+        self.burnRate = (-1) * self.massDot / (self.burnArea * self.grainDensity)
+        self.burnRate.setOutputs("Burn Rate (m/s)")
+        return self.burnRate
+
+    def evaluateKn(self):
         KnSource = (
             np.concatenate(
                 (
                     [self.grainInnerRadius.source[:, 1]],
-                    [self.burnArea.source[:, 1] / throatArea],
+                    [self.burnArea.source[:, 1] / self.throatArea],
                 )
             ).transpose()
         ).tolist()
         self.Kn = Function(
             KnSource,
             "Grain Inner Radius (m)",
             "Kn (m2/m2)",
             self.interpolate,
             "constant",
         )
-        # Burn Rate
-        self.burnRate = (-1) * self.massDot / (self.burnArea * self.grainDensity)
-        self.burnRate.setOutputs("Burn Rate (m/s)")
-
-        return [self.grainInnerRadius, self.grainHeight]
+        return self.Kn
 
     def evaluateInertia(self):
         """Calculates propellant inertia I, relative to directions
         perpendicular to the rocket body axis and its time derivative
         as a function of time. Also calculates propellant inertia Z,
         relative to the axial direction, and its time derivative as a
         function of time. Products of inertia are assumed null due to
@@ -561,19 +585,19 @@
         grainInertiaI = grainMass * (
             (1 / 4) * (self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2)
             + (1 / 12) * self.grainHeight ** 2
         )
 
         # Calculate each grain's distance d to propellant center of mass
         initialValue = (grainNumber - 1) / 2
-        d = np.linspace(-initialValue, initialValue, self.grainNumber)
+        d = np.linspace(-initialValue, initialValue, grainNumber)
         d = d * (self.grainInitialHeight + self.grainSeparation)
 
         # Calculate inertia for all grains
-        self.inertiaI = grainNumber * (grainInertiaI) + grainMass * np.sum(d ** 2)
+        self.inertiaI = grainNumber * grainInertiaI + grainMass * np.sum(d ** 2)
         self.inertiaI.setOutputs("Propellant Inertia I (kg*m2)")
 
         # Inertia I Dot
         # Calculate each grain's inertia I dot
         grainInertiaIDot = (
             grainMassDot
             * (
@@ -582,33 +606,31 @@
             )
             + grainMass
             * ((1 / 2) * self.grainInnerRadius - (1 / 3) * self.grainHeight)
             * self.burnRate
         )
 
         # Calculate inertia I dot for all grains
-        self.inertiaIDot = grainNumber * (grainInertiaIDot) + grainMassDot * np.sum(
+        self.inertiaIDot = grainNumber * grainInertiaIDot + grainMassDot * np.sum(
             d ** 2
         )
         self.inertiaIDot.setOutputs("Propellant Inertia I Dot (kg*m2/s)")
 
         # Inertia Z
         self.inertiaZ = (
             (1 / 2.0)
             * self.mass
             * (self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2)
         )
         self.inertiaZ.setOutputs("Propellant Inertia Z (kg*m2)")
 
         # Inertia Z Dot
-        self.inertiaZDot = (
-            (1 / 2.0) * (self.massDot * self.grainOuterRadius ** 2)
-            + (1 / 2.0) * (self.massDot * self.grainInnerRadius ** 2)
-            + self.mass * self.grainInnerRadius * self.burnRate
-        )
+        self.inertiaZDot = (1 / 2.0) * self.massDot * (
+            self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2
+        ) + self.mass * self.grainInnerRadius * self.burnRate
         self.inertiaZDot.setOutputs("Propellant Inertia Z Dot (kg*m2/s)")
 
         return [self.inertiaI, self.inertiaZ]
 
     def importEng(self, fileName):
         """Read content from .eng file and process it, in order to
         return the comments, description and data points.
@@ -628,29 +650,30 @@
             Description of the motor. All attributes are returned separated in
             a list. E.g. "F32 24 124 5-10-15 .0377 .0695 RV\n" is return as
             ['F32', '24', '124', '5-10-15', '.0377', '.0695', 'RV\n']
         dataPoints: list
             List of all data points in file. Each data point is an entry in
             the returned list and written as a list of two entries.
         """
-        # Intiailize arrays
+        # Initialize arrays
         comments = []
         description = []
         dataPoints = [[0, 0]]
 
         # Open and read .eng file
         with open(fileName) as file:
             for line in file:
-                if line[0] == ";":
+                if re.search(r";.*", line):
                     # Extract comment
-                    comments.append(line)
-                else:
+                    comments.append(re.findall(r";.*", line)[0])
+                    line = re.sub(r";.*", "", line)
+                if line.strip():
                     if description == []:
                         # Extract description
-                        description = line.split(" ")
+                        description = line.strip().split(" ")
                     else:
                         # Extract thrust curve data points
                         time, thrust = re.findall(r"[-+]?\d*\.\d+|[-+]?\d+", line)
                         dataPoints.append([float(time), float(thrust)])
 
         # Return all extract content
         return comments, description, dataPoints
@@ -674,28 +697,27 @@
         """
         # Open file
         file = open(fileName, "w")
 
         # Write first line
         file.write(
             motorName
-            + " {:3.1f} {:3.1f} 0 {:2.3} {:2.3} PJ \n".format(
+            + " {:3.1f} {:3.1f} 0 {:2.3} {:2.3} RocketPy\n".format(
                 2000 * self.grainOuterRadius,
                 1000
                 * self.grainNumber
                 * (self.grainInitialHeight + self.grainSeparation),
                 self.propellantInitialMass,
                 self.propellantInitialMass,
             )
         )
 
         # Write thrust curve data points
-        for item in self.thrust.source[:-1, :]:
-            time = item[0]
-            thrust = item[1]
+        for time, thrust in self.thrust.source[1:-1, :]:
+            # time, thrust = item
             file.write("{:.4f} {:.3f}\n".format(time, thrust))
 
         # Write last line
         file.write("{:.4f} {:.3f}\n".format(self.thrust.source[-1, 0], 0))
 
         # Close file
         file.close()
```

### Comparing `rocketpy-0.9.8/rocketpy/__init__.py` & `rocketpy-0.9.9/rocketpy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 design and trajectory optimization and dispersion analysis.
 """
 
 __author__ = "Giovani Hidalgo Ceotto"
 __copyright__ = "Copyright 20XX, Projeto Jupiter"
 __credits__ = ["Matheus Marques Araujo", "Rodrigo Schmitt", "Guilherme Tavares"]
 __license__ = "MIT"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __maintainer__ = "Giovani Hidalgo Ceotto"
 __email__ = "ghceotto@gmail.com"
 __status__ = "Production"
 
 import re
 import math
 import bisect
@@ -37,7 +37,8 @@
 from matplotlib import cm
 
 from .Function import Function
 from .Environment import Environment
 from .SolidMotor import SolidMotor
 from .Rocket import Rocket
 from .Flight import Flight
+from .utilities import *
```

### Comparing `rocketpy-0.9.8/rocketpy.egg-info/PKG-INFO` & `rocketpy-0.9.9/rocketpy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,352 +1,344 @@
-Metadata-Version: 2.1
-Name: rocketpy
-Version: 0.9.8
-Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/giovaniceotto/RocketPy
-Author: Giovani Hidalgo Ceotto
-Author-email: ghceotto@gmail.com
-Maintainer: RocketPy Developers
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://rocketpyalpha.readthedocs.io/en/latest/?badge=latest)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)
-[![Downloads](https://pepy.tech/badge/rocketpyalpha)](https://pepy.tech/project/rocketpyalpha)
-[![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
-
-# RocketPy
-RocketPy is a trajectory simulation for High-Power Rocketry built by [Projeto Jupiter](https://www.facebook.com/ProjetoJupiter/). The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
-
-### Main features
-
-<details>
-<summary>Nonlinear 6 degrees of freedom simulations</summary>
-<ul>
-  <li>Rigorous treatment of mass variation effects</li>
-  <li>Solved using LSODA with adjustable error tolerances</li>
-  <li>Highly optimized to run fast</li>
-</ul>
-</details>
-
-<details>
-<summary>Accurate weather modeling</summary>
-<ul>
-  <li>International Standard Atmosphere (1976)</li>
-  <li>Custom atmospheric profiles</li>
-  <li>Soundings (Wyoming, NOAARuc)</li>
-  <li>Weather forecasts and reanalysis</li>
-  <li>Weather ensembles</li>
-</ul>
-</details>
-
-<details>
-<summary>Aerodynamic models</summary>
-<ul>
-  <li>Barrowman equations for lift coefficients (optional)</li>
-  <li>Drag coefficients can be easily imported from other sources (e.g. CFD simulations)</li>
-</ul>
-</details>
-
-<details>
-<summary>Parachutes with external trigger functions</summary>
-<ul>
-  <li>Test the exact code that will fly</li>
-  <li>Sensor data can be augmented with noise</li>
-</ul>
-</details>
-
-<details>
-<summary>Solid motors models</summary>
-<ul>
-  <li>Burn rate and mass variation properties from thrust curve</li>
-  <li>CSV and ENG file support</li>
-</ul>
-</details>
-
-<details>
-<summary>Monte Carlo simulations</summary>
-<ul>
-  <li>Dispersion analysis</li>
-  <li>Global sensitivity analysis</li>
-</ul>
-</details>
-
-<details>
-<summary>Flexible and modular</summary>
-<ul>
-  <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
-  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
-  <li>Multi-stage rockets</li>
-  <li>Custom continuous and discrete control laws</li>
-  <li>Create new classes (e.g. other types of motors)</li>
-</ul>
-</details>
-
-### Documentation
-
-Check out documentation details using the links below:
-  - [User Guide](https://rocketpyalpha.readthedocs.io/en/latest/user/index.html)
-  - [Code Documentation](https://rocketpyalpha.readthedocs.io/en/latest/reference/index.html)
-  - [Development Guide](https://rocketpyalpha.readthedocs.io/en/latest/development/index.html)
-
-## Join Our Community!
-RocketPy is growing fast! Many unviersity groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
-
-If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
-
-## Previewing
-
-You can preview RocketPy's main functionalities by browsing through a sample notebook either in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb) or in [MyBinder](https://mybinder.org/v2/gh/giovaniceotto/RocketPy/master?filepath=docs%2Fnotebooks%2Fgetting_started.ipynb)!
-
-Then, you can read the *Getting Started* section to get your own copy!
-
-## Getting Started
-
-These instructions will get you a copy of RocketPy up and running on your local machine.
-
-### Prerequisites
-
-The following is needed in order to run RocketPy:
-
- - Python >= 3.0
- - Numpy >= 1.0
- - Scipy >= 1.0
- - Matplotlib >= 3.0
- - requests
- - netCDF4 >= 1.4 (optional, requires Cython)
- 
-All of these packages, with the exception of netCDF4, should be automatically
-installed when RocketPy is installed using either pip or conda.
-
-However, in case the user wants to install these packages manually, they can do
-so by following the instructions bellow:
-
-The first 4 prerequisites come with Anaconda, but Scipy might need
-updating. The nedCDF4 package can be installed if there is interest in
-importing weather data from netCDF files. To update Scipy and install
-netCDF4 using Conda, the following code is used:
-
-```
-$ conda install "scipy>=1.0"
-$ conda install -c anaconda "netcdf4>=1.4"
-```
-
-Alternatively, if you only have Python 3.X installed, the packages needed can be installed using pip:
-
-```
-$ pip install "numpy>=1.0"
-$ pip install "scipy>=1.0"
-$ pip install "matplotlib>=3.0"
-$ pip install "netCDF4>=1.4"
-$ pip install "requests"
-```
-
-Although [Jupyter Notebooks](http://jupyter.org/) are by no means required to run RocketPy, they are strongly recommend. They already come with Anaconda builds, but can also be installed separately using pip:
-
-```
-$ pip install jupyter
-```
-
-### Installation
-
-To get a copy of RocketPy using pip, just run:
-
-```
-$ pip install rocketpyalpha
-```
-
-Alternatively, the package can also be installed using conda:
-
-```
-$ conda install -c conda-forge rocketpy
-```
-
-If you want to downloaded it from source, you may do so either by:
-
-- Downloading it from [RocketPy's GitHub](https://github.com/giovaniceotto/RocketPy) page
-    - Unzip the folder and you are ready to go
-- Or cloning it to a desired directory using git:
-    - ```$ git clone https://github.com/giovaniceotto/RocketPy.git```
-
-The RockeyPy library can then be installed by running:
-
-```
-$ python setup.py install 
-```
-
-### Documentations
-
-You can find RocketPy's documentation at [Read the Docs](https://rocketpyalpha.readthedocs.io/en/latest/).
-
-### Running Your First Simulation
-
-In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the **_nbks_** folder. Open **_Getting Started - Examples.ipynb_** and you are ready to go.
-
-Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
-
-- Environment - Keeps data related to weather.
-- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
-- Rocket - Keeps data related to a rocket.
-- Flight - Runs the simulation and keeps the results.
-
-A typical workflow starts with importing these classes from RocketPy:
-
-```python
-from rocketpy import Environment, Rocket, SolidMotor, Flight
-```
-
-Then create an Environment object. To learn more about it, you can use:
-
-```python
-help(Environment)
-```
-
-A sample code is:
-
-```python
-Env = Environment(
-    railLength=5.2,
-    latitude=32.990254,
-    longitude=-106.974998,
-    elevation=1400,
-    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
-) 
-
-Env.setAtmosphericModel(type='Forecast', file='GFS')
-```
-
-This can be followed up by starting a Solid Motor object. To get help on it, just use:
-
-```python
-help(SolidMotor)
-```
-
-A sample Motor object can be created by the following code:
-
-```python
-Pro75M1670 = SolidMotor(
-    thrustSource="../data/motors/Cesaroni_M1670.eng",
-    burnOut=3.9,
-    grainNumber=5,
-    grainSeparation=5/1000,
-    grainDensity=1815,
-    grainOuterRadius=33/1000,
-    grainInitialInnerRadius=15/1000,
-    grainInitialHeight=120/1000,
-    nozzleRadius=33/1000,
-    throatRadius=11/1000,
-    interpolationMethod='linear'
-)
-```
-
-With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
-
-```python
-help(Rocket)
-```
-
-A sample code to create a Rocket is:
-
-```python
-Calisto = Rocket(
-    motor=Pro75M1670,
-    radius=127/2000,
-    mass=19.197-2.956,
-    inertiaI=6.60,
-    inertiaZ=0.0351,
-    distanceRocketNozzle=-1.255,
-    distanceRocketPropellant=-0.85704,
-    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
-    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
-)
-
-Calisto.setRailButtons([0.2, -0.5])
-
-NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
-
-FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
-
-Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
-```
-
-You may want to add parachutes to your rocket as well:
-
-```python
-def drogueTrigger(p, y):
-    return True if y[5] < 0 else False
-
-def mainTrigger(p, y):
-    return True if y[5] < 0 and y[2] < 800 else False
-
-Main = Calisto.addParachute('Main',
-                            CdS=10.0,
-                            trigger=mainTrigger, 
-                            samplingRate=105,
-                            lag=1.5,
-                            noise=(0, 8.3, 0.5))
-
-Drogue = Calisto.addParachute('Drogue',
-                              CdS=1.0,
-                              trigger=drogueTrigger, 
-                              samplingRate=105,
-                              lag=1.5,
-                              noise=(0, 8.3, 0.5))
-```
-
-Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
-
-```python
-help(Flight)
-```
-
-To actually create a Flight object, use:
-
-```python
-TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
-```
-
-Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
-
-```python
-TestFlight.info()
-```
-
-To seel all available results, use:
-
-```python
-TestFlight.allInfo()
-```
-
-## Built With
-
-* [Numpy](http://www.numpy.org/)
-* [Scipy](https://www.scipy.org/)
-* [Matplotlib](https://matplotlib.org/)
-* [netCDF4](https://github.com/Unidata/netcdf4-python)
-
-## Contributing
-
-Please read [CONTRIBUTING.md](https://github.com/giovaniceotto/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us. - **_Still working on this!_**
-
-## Authors
-
-* Creator: **Giovani Hidalgo Ceotto**
-
-See the list of [contributors](https://github.com/giovaniceotto/RocketPy/contributors) who are actively working on RocketPy.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/giovaniceotto/RocketPy/blob/master/LICENSE) file for details
-
-## Release Notes
-Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/giovaniceotto/RocketPy/releases).
-
-
-
+Metadata-Version: 2.1
+Name: rocketpy
+Version: 0.9.9
+Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
+Home-page: https://github.com/giovaniceotto/RocketPy
+Author: Giovani Hidalgo Ceotto
+Author-email: ghceotto@gmail.com
+Maintainer: RocketPy Developers
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![RocketPy Logo](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
+
+<br>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
+[![PyPI](https://img.shields.io/pypi/v/rocketpy?color=g)](https://pypi.org/project/rocketpy/)
+[![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://docs.rocketpy.org/en/latest/?badge=latest)
+[![Build Status](https://app.travis-ci.com/Projeto-Jupiter/RocketPy.svg?branch=master)](https://app.travis-ci.com/Projeto-Jupiter/RocketPy)
+[![Contributors](https://img.shields.io/github/contributors/Projeto-Jupiter/rocketpy)](https://github.com/Projeto-Jupiter/RocketPy/graphs/contributors)
+[![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/rocketpy)
+[![DOI](https://img.shields.io/badge/DOI-10.1061%2F%28ASCE%29AS.1943--5525.0001331-blue.svg)](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331)
+
+<img src="https://static.scarf.sh/a.png?x-pxid=6f4094ab-00fa-4a8d-9247-b7ed27e7164d" />
+
+# RocketPy
+RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
+
+<br>
+
+## Main features
+<details>
+<summary>Nonlinear 6 degrees of freedom simulations</summary>
+<ul>
+  <li>Rigorous treatment of mass variation effects</li>
+  <li>Solved using LSODA with adjustable error tolerances</li>
+  <li>Highly optimized to run fast</li>
+</ul>
+</details>
+
+<details>
+<summary>Accurate weather modeling</summary>
+<ul>
+  <li>International Standard Atmosphere (1976)</li>
+  <li>Custom atmospheric profiles</li>
+  <li>Soundings (Wyoming, NOAARuc)</li>
+  <li>Weather forecasts and reanalysis</li>
+  <li>Weather ensembles</li>
+</ul>
+</details>
+
+<details>
+<summary>Aerodynamic models</summary>
+<ul>
+  <li>Barrowman equations for lift coefficients (optional)</li>
+  <li>Drag coefficients can be easily imported from other sources (e.g. CFD simulations)</li>
+</ul>
+</details>
+
+<details>
+<summary>Parachutes with external trigger functions</summary>
+<ul>
+  <li>Test the exact code that will fly</li>
+  <li>Sensor data can be augmented with noise</li>
+</ul>
+</details>
+
+<details>
+<summary>Solid motors models</summary>
+<ul>
+  <li>Burn rate and mass variation properties from thrust curve</li>
+  <li>CSV and ENG file support</li>
+</ul>
+</details>
+
+<details>
+<summary>Monte Carlo simulations</summary>
+<ul>
+  <li>Dispersion analysis</li>
+  <li>Global sensitivity analysis</li>
+</ul>
+</details>
+
+<details>
+<summary>Flexible and modular</summary>
+<ul>
+  <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
+  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
+  <li>Multi-stage rockets</li>
+  <li>Custom continuous and discrete control laws</li>
+  <li>Create new classes (e.g. other types of motors)</li>
+</ul>
+</details>
+
+<br>
+
+## Validation
+
+RocketPy's features have been validated in our latest [research article published in the Journal of Aerospace Engineering](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331).
+
+The table below shows a comparison between experimental data and the output from RocketPy.
+Flight data and rocket parameters used in this comparison were kindly provided by [EPFL Rocket Team](https://github.com/EPFLRocketTeam) and [Notre Dame Rocket Team](https://ndrocketry.weebly.com/).
+
+|         Mission         |    Result Paramater    | RocketPy  | Measured  | Relative Error |
+|:-----------------------:|:-----------------------|:---------:|:---------:|:--------------:|
+|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**   |
+|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**   |
+|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **4.24 %**   |
+|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**  |
+|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**  |
+|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**   |
+
+<br>
+
+## Documentation
+
+Check out documentation details using the links below:
+
+  - [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
+  - [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
+  - [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
+
+<br>
+
+# Join Our Community!
+RocketPy is growing fast! Many university groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
+
+If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
+
+<br>
+
+# Previewing
+
+You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb).  No installation required!
+
+When you are ready to run RocketPy locally, you can read the *Getting Started* section!
+
+<br>
+
+# Getting Started
+
+## Quick Installation
+
+To install RocketPy's latest stable version from PyPI, just open up your terminal and run:
+
+```shell
+pip install rocketpy
+```
+
+For other installation options, visit our [Installation Docs](https://docs.rocketpy.org/en/latest/user/installation.html).
+To learn more about RocketPy's requirements, visit our [Requirements Docs](https://docs.rocketpy.org/en/latest/user/requirements.html).
+
+<br>
+
+## Running Your First Simulation
+
+In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _nbks_ folder. Open _Getting Started - Examples.ipynb_ and you are ready to go.
+
+Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
+
+- Environment - Keeps data related to weather.
+- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
+- Rocket - Keeps data related to a rocket.
+- Flight - Runs the simulation and keeps the results.
+
+The following image shows how the four main classes interact with each other:
+
+![Diagram](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
+
+A typical workflow starts with importing these classes from RocketPy:
+
+```python
+from rocketpy import Environment, Rocket, SolidMotor, Flight
+```
+
+Then create an Environment object. To learn more about it, you can use:
+
+```python
+help(Environment)
+```
+
+A sample code is:
+
+```python
+Env = Environment(
+    railLength=5.2,
+    latitude=32.990254,
+    longitude=-106.974998,
+    elevation=1400,
+    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
+) 
+
+Env.setAtmosphericModel(type='Forecast', file='GFS')
+```
+
+This can be followed up by starting a Solid Motor object. To get help on it, just use:
+
+```python
+help(SolidMotor)
+```
+
+A sample Motor object can be created by the following code:
+
+```python
+Pro75M1670 = SolidMotor(
+    thrustSource="../data/motors/Cesaroni_M1670.eng",
+    burnOut=3.9,
+    grainNumber=5,
+    grainSeparation=5/1000,
+    grainDensity=1815,
+    grainOuterRadius=33/1000,
+    grainInitialInnerRadius=15/1000,
+    grainInitialHeight=120/1000,
+    nozzleRadius=33/1000,
+    throatRadius=11/1000,
+    interpolationMethod='linear'
+)
+```
+
+With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
+
+```python
+help(Rocket)
+```
+
+A sample code to create a Rocket is:
+
+```python
+Calisto = Rocket(
+    motor=Pro75M1670,
+    radius=127/2000,
+    mass=19.197-2.956,
+    inertiaI=6.60,
+    inertiaZ=0.0351,
+    distanceRocketNozzle=-1.255,
+    distanceRocketPropellant=-0.85704,
+    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
+    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
+)
+
+Calisto.setRailButtons([0.2, -0.5])
+
+NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
+
+FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
+
+Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
+```
+
+You may want to add parachutes to your rocket as well:
+
+```python
+def drogueTrigger(p, y):
+    return True if y[5] < 0 else False
+
+def mainTrigger(p, y):
+    return True if y[5] < 0 and y[2] < 800 else False
+
+Main = Calisto.addParachute('Main',
+                            CdS=10.0,
+                            trigger=mainTrigger, 
+                            samplingRate=105,
+                            lag=1.5,
+                            noise=(0, 8.3, 0.5))
+
+Drogue = Calisto.addParachute('Drogue',
+                              CdS=1.0,
+                              trigger=drogueTrigger, 
+                              samplingRate=105,
+                              lag=1.5,
+                              noise=(0, 8.3, 0.5))
+```
+
+Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
+
+```python
+help(Flight)
+```
+
+To actually create a Flight object, use:
+
+```python
+TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
+```
+
+Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
+
+```python
+TestFlight.info()
+```
+
+To seel all available results, use:
+
+```python
+TestFlight.allInfo()
+```
+
+Here is just a quick taste of what RocketPy is able to calculate. There are hundred of plots and data points computed by RocketPy to enhance your analyses.
+
+![6-DOF Trajectory Plot](docs/static/rocketpy_example_trajectory.svg)
+
+<br>
+
+# Authors and Contributors
+
+This package was originally created by [Giovani Ceotto](https://github.com/giovaniceotto/) as part of his work at [Projeto Jupiter](https://github.com/Projeto-Jupiter/). [Rodrigo Schmitt](https://github.com/rodrigo-schmitt/) was one of the first contributors.
+
+Later, [Guilherme Fernandes](https://github.com/Gui-FernandesBR/) and [Lucas Azevedo](https://github.com/lucasfourier/) joined the team to work on the expansion and sustainability of this project.
+
+Since then, the [RocketPy Team](https://github.com/orgs/Projeto-Jupiter/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
+
+[![GitHub Contributors Image](https://contrib.rocks/image?repo=Projeto-Jupiter/RocketPy)](https://github.com/Projeto-Jupiter/RocketPy/contributors)
+
+See a [detailed list of contributors](https://github.com/Projeto-Jupiter/RocketPy/contributors) who are actively working on RocketPy.
+
+## Supporting RocketPy and Contributing
+
+The easiest way to help RocketPy is to demonstrate your support by starring our repository! ![GitHub Repo stars](https://img.shields.io/github/stars/Projeto-Jupiter/RocketPy?style=social)
+
+<br>
+
+If you are actively using RocketPy in one of your projects, reaching out to our core team via [Discord](https://discord.gg/b6xYnNh) and providing feedback can help improve RocketPy a lot!
+
+And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more on how you can contribute with the development of this next-gen trajectory simulation solution for rocketry.
+
+<br>
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/LICENSE) file for details
+
+<br>
+
+## Release Notes
+Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/Projeto-Jupiter/RocketPy/releases).
+
+
```

### Comparing `rocketpy-0.9.8/setup.py` & `rocketpy-0.9.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="rocketpy", 
-    version="0.9.8",
-    install_requires = [
-        'numpy>=1.0',
-        'scipy>=1.0',
-        'matplotlib>=3.0',
-        'requests'
-    ],
+    name="rocketpy",
+    version="0.9.9",
+    install_requires=["numpy>=1.0", "scipy>=1.0", "matplotlib>=3.0", "requests"],
     maintainer="RocketPy Developers",
     author="Giovani Hidalgo Ceotto",
     author_email="ghceotto@gmail.com",
     description="Advanced 6-DOF trajectory simulation for High-Power Rocketry.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/giovaniceotto/RocketPy",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

