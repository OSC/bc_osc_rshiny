# [WIP] Batch Connect - OSC Shiny App Launcher

![GitHub Release](https://img.shields.io/github/release/osc/shiny_launcher.svg)
[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

A Batch Connect app designed for OSC OnDemand that launches a Shiny App within
an Owens batch job.

The Shiny app is included a submodule and each deployment can modified which
Shiny app to deploy using git config to specify the URL for the submodule. This
way the launcher code can be reused for multiple apps but the launcher and the
app itself can be managed separately.

## Prerequisites

This Batch Connect app requires the following software be installed on the
**compute nodes** that the batch job is intended to run on (**NOT** the
OnDemand node):

- [Shiny] x.y.z+
- [Lmod] 6.0.1+ or any other `module purge` and `module load <modules>` based
  CLI used to load appropriate environments within the batch job

[Shiny]: https://shiny.rstudio.com/
[Lmod]: https://www.tacc.utexas.edu/research-development/tacc-projects/lmod

## Install

**TODO**

Again, you do not need to restart the app as it isn't a Passenger app.

## Contributing

1. Fork it ( https://github.com/OSC/bc_osc_example_shiny/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
