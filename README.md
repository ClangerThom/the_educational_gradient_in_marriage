## How to use this replication script:

1. Edit the config.R file to add file paths to data and all your outputs like tables and figures. I did this because the data files were large and I needed to sync them via Onedrive. I don't have my github projects on the Onedrive.
2. Download all GGS data from https://www.ggp-i.org/ after getting access to it. Rename Harmonized Histories files to "harmonized_histories.dta", "harmonized_histories_I.dta", and "harmonized_histories_II.dta". For manual harmonization download the French, Dutch, and Swedish round 2 files and rename them to "france_round2.dta", "netherlands_round2.dta", and "sweden_round2.dta". You have to use the .dta Stata files. Later rounds had .csv files available, but older ones were just in Stata or SPSS format so for my own ease of use I just went the stata files everywhere.
3. Run the harmonization script.
4. Run the data_cleaning script.
5. Run the code blocs in the analysis script up to and including creation of country-cohorts and analytical sample
6. Run macro_data_cleaning
7. Run the rest of the analysis script

Note: I optimised the script to run a little faster in the analysis. Nonetheless, make sure you don't try to replicate this on a machine that has less than 16gb of RAM and a slow processor. The script either won't have enough memory to even execute or you will get stuck for a VERY long time trying to run it.
