
<!-- README.md is generated from README.Rmd. Please edit that file -->

# shinySbm

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

`shinySbm` is a package containing a shiny application. This application
is build for network analysis based on the `sbm` package made by Chiquet
J, Donnet S and Barbillon P (2023)
[CRAN](https://CRAN.R-project.org/package=sbm). It allow to apply and
explore the outputs of a Stochastic Block Model. It is useful if you
want to analyse your data (could be adjacency matrix or edges list)
without `R` language knowledge or to learn the basic lines of the `sbm`
package.

The Stochastic Block Model is applied on network to simplify the
information they gather, and help to visualize the main
behaviours/categories/relations there is in your network. It’s a latent
model which identify significant groups with similar behaviour by
gathering the network nodes. By this you could be able to know if your
network is : hidding closed sub-communities, hierachized, or is having
another specific structure.

With this application you should be also able to :

- Easyly run a Stochastic Block Model
- Get some nice outputs as matrix and network plots organized by groups
- Get a modelisation summary
- Extract nodes lists associated with their groups

## How to use the Application

### With `R`

#### Installation

You can install the development version of shinySbm like so:

``` r
remotes::install_github("Jo-Theo/shinySbm")
```

The shinySbm package should be installed.

#### Running The Application

From a new `R` session you can then run

``` r
shinySbm::run_app()
```

### With `docker`

#### Installation

If you are familiar to `docker`, you can also download the docker image
by running the command :

``` bash
docker pull registry.forgemia.inra.fr/theodore.vanrenterghem/shinysbm:latest
```

#### Running The Application

Once installed you can run the command to launch the app :

``` bash
docker run -p 3838:3838 registry.forgemia.inra.fr/theodore.vanrenterghem/shinysbm:latest
```

And then from your browser find the address `http://localhost:3838/`

## Contact

Any questions, problems or comments regarding this application ? Contact
us : [shiny.sbm.dev@gmail.com](shiny.sbm.dev@gmail.com)

## References

Chiquet J, Donnet S, Barbillon P (2023). sbm: Stochastic Blockmodels. R
package version 0.4.5,  
<https://CRAN.R-project.org/package=sbm>.
