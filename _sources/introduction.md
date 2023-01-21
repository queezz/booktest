---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Humanity and Energy

# World's energy consumption
## From a cell to a powerplant
The whole of humanity relies on energy. In fact, all biological systems, from small to big, are determined by their energy production.
For instance, in the transition from a simple bacteria to a multicellular life, a symbiosis of two organisms happend. Bacteria can only produce energy on it's surface, but the energy is consumend in it's volume. Increasing energy production means increasing it's surface, however at some point this becomes not valiable, because the volume grows as $r^3$, and the surface - as $r^2$ (for a "spherical" bacterium). But if one cell could host several specified power producing cels inside it, then this limitation could be overcome. Thus mitochondria inside a eukaryotic cell allowed exactly that. And with so much increased energy production, suddenly, a whole range of new possibilities arrived: a colony of single cells formed a multicellural organisms.  

Our society is a new chapter in the energy race of life. Most of human progress could be easily linked with humanity's ability to produce energy. And now we are facing a barrier. Most of the easy-to-get fuels are almost used up, but the world's consumption grows and grows. How to deal with such situation? And what is the situation? 

Let's take a look at [Robert J. Goldston](https://thebulletin.org/2018/04/why-fusion-2/) paper, specifically at the IPCC projected worldwide annually averaged electrical power production, GWe (gigawatts electric).

| Source     | 2020  | 2050  | 2100  |
| :--------- | :---: | :---: | :---: |
| Solar      |  30   |  650  | 3720  |
| Nuclear    |  400  | 1120  | 2230  |
| Wind       |  150  |  930  | 2170  |
| Biomass    |  40   |  540  | 1500  |
| Hydro      |  410  |  640  |  850  |
| Coal + Oil |  920  |  860  |  770  |
| Gas        |  780  |  980  |  620  |
| Geothermal |  30   |  84   |  100  |
| Total      | 2770  | 5800  | 11900 |

Or, if we put it into a plot:

```{code-cell}
:tags: ["hide-input"]

import matplotlib.pyplot as plt
names = ['Solar', 'Nuclear', 'Wind', 'Biomass', 'Hydro', 'Coal + Oil', 'Gas', 'Geothermal', 'Total']
p2020 = [30,  400,  150,   40,  410,  920,  780,   30, 2770]
p2050 = [650, 1120,  930,  540,  640,  860,  980,   84, 5800]
p2100 = [3720,  2230,  2170,  1500,   850,   770,   620,   100, 11900]
plt.plot(p2020,'o--',label='2020')
plt.plot(p2050,'^-',label='2050')
plt.plot(p2100,'s-.',label='2100')
plt.yscale('log')
plt.legend()
plt.ylabel('Power Production, GW')

_ = plt.xticks(list(range(len(names))),names,rotation=90)
```

Maybe this is a bit of a pessimistic project for nuclear power production increase and overly optimistic for solar and wind, but it's a projection for 80 years into the future, so it must be wrong.

# Magnetic confinement.
Tokamaks vs stellarators from [IAEA](https://www.iaea.org/bulletin/magnetic-fusion-confinement-with-tokamaks-and-stellarators).

|                             tokamak                              |                             stellarator                             |
| :--------------------------------------------------------------: | :-----------------------------------------------------------------: |
| ![Tokamak](https://www.iaea.org/sites/default/files/tokamak.png) | ![Tokamak](https://www.iaea.org/sites/default/files/stellartor.png) |

Tokamaks are a promissing concept for future fusion power plants, but not everybody agrees, as Daniel Jassby writes in [his article](https://thebulletin.org/2017/04/fusion-reactors-not-what-theyre-cracked-up-to-be/).


```{epigraph}
By way of comparison, in the two magnetic confinement fusion facilities where tritium has been used (Princeton’s Tokamak Fusion Test Reactor, and the Joint European Torus), approximately 10 percent of the injected tritium was never recovered {cite:p}`TANABE2003478`.

-- Daniel Jassby
```



```{bibliography}
:filter: docname in docnames
```