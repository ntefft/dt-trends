# lp: Estimating the prevalence and relative risk of drinking drivers

This repo contains scripts implementing the estimation methods developed by Levitt and Porter (2001), hereafter LP. The scripts allow for direct download and extraction of the raw data from the Fatality Analysis Reporting System (from the NHTSA), estimation of the maximum likelihood model, and replication of LP.

To replicate LP, run the following scripts, in order:
1. retrieve.py to retrieve and save the raw data from NHTSA's FTP site.
2. extract.py (in the "replication" folder) to extract and harmonize relevant estimation variables across survey years. The combined accident, vehicle, and person files are then stored in the replication\data folder.
3. replicate.py (in the "replication" folder) to generate summary statistics and estimation results that replicate LP.

Projects similar to the "replication" project may be generated, using the underlying data and coded estimation methods (which are contained in estimate.py). To maintain file organization, it is recommended that the user create a copy of the "replication" folder, rename it, and then edit the contained scripts for their new project. 

References
Levitt, Steven D., and Jack Porter. How Dangerous are Drinking Drivers? Journal of Political Economy, 2001, 109(6), pgs. 1198-1237.
