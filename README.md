
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rtaxref – an R client to the French Taxonomical Reference

[![Project Status: WIP – Initial development is in progress, but there
has not yet been a stable, usable release suitable for the
public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

The goal of rtaxref is to provide an R client to TaxRef, the French
Taxonomical Reference.

## Installation

You can install the development version of rtaxref from GitHub with:

``` r
remotes::install_github("Rekyt/rtaxref")
```

## Using `rtaxref`

For the moment `rtaxref` only contains function to interact with TaxRef
on taxon’s name and id.

`rt_taxa_search()` let’s you search a taxon with different criteria:

``` r
rt_taxa_search(sciname = "Helianthus annuus")
```

Other taxa functions `rt_taxa_children()`, `rt_taxa_id()`,
`rt_taxa_parent()`, `rt_taxa_taxrefhistory()`, all use a single argument
`id` to retrieve their data. The `id` is the unique identifier of the
taxa in TaxRef and is also called `cdNom`.

``` r
rt_taxa_id(id = 101027)
```
