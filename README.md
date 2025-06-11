#pb-level-detector

A python script that cleans and formats messy lead surveillance data for better analysis.

This is a GUI tool that reads, analyzes, and flags elevated lead levels in environmental or clinical datasets.This project was inspired by my work at the Maryland Department of the Environment (MDE), where I supported the Lead Poisoning Prevention Program, Surveillance Unit. 

Example

If you upload this:

| Name         | Address                                     | Lead Level |
|--------------|---------------------------------------------|------------|
| Jack the Ripper     | 100 N Holliday St, Baltimore, MD            | 4.2        |

You’ll get this:

| Name         | Address                   | Lead Level | Lead Flag | Street Address | City      | State | Zip Code (from Address) |
|--------------|---------------------------|------------|-----------|----------------|-----------|-------|--------------------------|
| Jack the Ripper     | 100 N Holliday St, Baltimore, MD | 4.2        | High      | 100 N Holliday St    | Baltimore | MD    | 21202                   |

And the Lead Level and Lead Flag cells will be highlighted in **red**.
