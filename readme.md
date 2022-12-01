# Tree TSAR repo

## Quick notes on this repo
Files within the `_site` directory should be left alone, as they are the output files when the site builds. If we need to adjust a section, add a species, or edit a genus, that should all be done **outside** the _site directory. More information on jekyll directory structure can be found [here](https://jekyllrb.com/docs/structure/).
## Adding new species page within the repo on GitHub
Adding a new species page involves creating a new markdown file in the correct directory with the correct properties. For example, if we were missing the abies species, you would create a new file called `abies.markdown` within the `_pinaceae/_abies` directory.

## Required frontmatter for species pages
If adding a species on GitHub (from the section above) your markdown file must start with the following frontmatter:
```
---
species-name: alba
common-name: Silver fir
family-name: Pinaceae
genus-name: Abies
[IF APPLICABLE] infrageneric-level-I: Section Abies
[IF APPLICABLE] infrageneric-level-II: 
[IF APPLICABLE] infrageneric-level-III: 
[IF APPLICABLE] infrageneric-level-IV: 
layout: species
---
```
## Adding new species page within Forestry.io
Click `Create New` then select `Pages` within the genus the species lives. Fill out the required information to generate the page. Layout needs to be `species` as this is a species page.

## Building collections from data files into markdown files:
We can compile species pages via data by formatting .csv or .json and putting the files in the _data directory using [jekyll-pagemaster](https://github.com/mnyrop/pagemaster/#readme). From there ensure that the required properties are listed in the collection within `_config.yml`. 

example collection properties:
```
collections:
  abies:
    output: true
    family-name: Pinaceae
    genus-name: Abies
    source: abies-all.json
    id_key: species-name
    layout: species
    permalink: /trees/pinaceae/:collection/:name
```
example build command: `bundle exec jekyll pagemaster abies`