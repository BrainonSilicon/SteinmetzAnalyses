# Hello! 

This is the repo for some data analysis using the Open Source [Steinmetz Neuropixel Dataset](http://data.cortexlab.net/). The aim of this project is to roadtest different skill sets in an "open science" environment and be able to collaborate more freely. 

:brain: Dense arrays (the physical type) were used to record from mice during a go/no-go task. It's an incredibly rich dataset for understanding movement, decisions, visual processing (and lots more I haven't thought of). 

The easiest way to see what's in the data is to load it up and to read through the key labels on the dataset:

```
# choose one recording session (eg.20) to get labels
session_20 = steinmetz_data[20]
keys = session_20.keys()
print(keys)

```
Note: session 4 has really good Primary Visual Cortex data so that's always a good place to start. 

:mouse: You can read more about the neuropixel dataset [here](https://www.biorxiv.org/content/10.1101/2020.10.27.358291v1) 


## Goals

The project has 3 current objectives:

1. Use a [Binder](https://mybinder.org/) environment to write code openly and support learning (Binder is great for demos!)
2. Explore the absolutely awesome dataset from Steinmetz's team to learn more about neural processing
3. Continue learning and iterating over the code so that what took 20 lines, will eventually be done in 4



## Built With

The analyses use python and there is a jupyter notebook in case you prefer jupyter.

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)



## Get Started

:star2: There's a few entry point



## Tests

The jupyter notebook currently has tests implemented in the one file, however some next steps are to separate out the analyses and the tests. If you feel knowledgeable about this then feel free to open an issue! 
The goal is to move away from writing analyses just to publish a paper and towards good software pratices (such as TDD). 

Inline-style: 
![Good Code](https://imgs.xkcd.com/comics/good_code.png "Good Code from xkcd")


## Credits

This is all made possible because of the [Nick Steinmetz](http://www.nicksteinmetz.com/) and the Neuropixel researchers who have made this data available for use.


## License

[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
