# EN584 Cruise, June 2016

This repository contains scripts for calculating hydrolysis rates of polysaccharides (FLA) and short substrates (PlateReader)

## Plate Reader

Incubations of seawater with seven short organic substrates (monosaccharides and peptides) were conducted in 96-well plates for several experiments. Fluorescence was measured over time in the plates using a plate reader.
This folder contains scripts and reference files to calculate hydrolysis rates of those seven substrates.

Four types of incubations were conducted:
1) bulk seawater (bulk) - substrates amended to bulk seawater
2) Large Volume (LV) - seawater amended with algae extract in large carboys, incubations with substrates conducted at subsampling points of carboys
3) Gravity Filtration (GF) - filters containing particles (filtered from seawater) suspended in autoclaved seawater
4) Free Living (free) - filtrate from gravity filtration, containing only free living bacteria and no particles

This folder contains five R scripts:

* Plate_UpdateTimesheet_EN584.R - from a directory of plate reader output files (.xlsx), extract the time sampled, calculate the elapsed time (in hours) from the t0 sampling point. Output timesheet as a .csv file.

* rawToRatesEN584_bulk.R - calculate hydrolysis rates for all bulk incubations

* rawToRatesEN584_LV.R - calculate hydrolysis rates for all LV incubations

* rawToRatesEN584_GF.R - calculate hydrolysis rates for all GF incubations

* rawToRatesEN584_free.R - calculate hydrolysis rates for all free living incubations
