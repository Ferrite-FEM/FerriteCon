# FerriteCon webpage
The website can be found [here](https://ferrite-fem.github.io/FerriteCon), 
this readme provides instructions for how to update the webpage.

## Create the next edition
* Copy the last year's folder, rename to the current year, and update contents
* When ready to make the redirection so it becomes the landing page, change the 
  `url=` field in the top-level [`index.html`](/index.html).

## Preview locally
From the local [environment](/Project.toml), run
```julia
using Franklin
serve()
```
