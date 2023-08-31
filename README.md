# Setup

The codes for scraping and parsing were adapted from the original codes used in Pico et al. (2020). Installation instructions are copied from their repository.

## Basic setup instructions

First set up a virtual environment in the top level of this repo and
source it

```
$ virutalenv venv
```
```
$ source venv/bin/activate
```

Next, pip install the requirements.txt (note: this file is not updated!)

```
$ pip3 install -r requirements.txt
```

Now install a notebook kernel that will use this virtual environment

```
$ python -m ipykernel install --user --name=venv
```

Run the jupyter notebook server, and to use these notebooks select the
kernel named `venv` (or whatever you chose as a name).

## WebDriver

The webdriver we used with selenium is included in this repo under the
`deps` directory. It is compatible with Google Chrome versions 70-73.
Other versions of chromedrivers can be [downloaded here](https://chromedriver.chromium.org/downloads).


# Acknowledgments

The file `gender.py` is copied from [github.com/block8432/gender.py](https://github.com/block8437/gender.py)

# Citation

Please cite:

```
Pico, T., Bierman, P., Doyle, K., & Richardson, S. (2020). First authorship gender gap in the geosciences. Earth and Space Science, 7, e2020EA001203. https://doi.org/10.1029/2020EA001203 

Ermert, L. A., Koroni, M., and Korta Martiartu, N.: Quantifying gender gaps in seismology authorship, Solid Earth, 14, 485–498, https://doi.org/10.5194/se-14-485-2023, 2023
```

## overview of all the notebooks and scripts:

For collecting journal pages and parsing publication data use:

```
Scrape_Journals.ipynb
Parse_journal_data.ipynb

```

For downloading EGU abstract data:

```
ScrapeAndParse_EGUAbstractData.ipynb
```

For probabilistic analysis:

```
analysis-clean.ipynb 
conditional_probabilities_teamcomposition.ipynb
```

