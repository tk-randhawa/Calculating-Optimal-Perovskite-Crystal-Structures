# File Information

## Summary:
- This work was done during Summer 2021 as a part of the Leadership Alliance Summer Research-Early Identification Program. All of the research was conducted at the Stanford University Department of Chemistry
- Project is a continuation of https://pubs.rsc.org/en/content/articlelanding/2021/sc/d1sc01159f (DOI: 10.1039/d1sc01159f)
- Background information & project summary can be found on the "Final Presentation.pdf" file in this repo (https://github.com/tk-randhawa/Calculating-Optimal-Perovskite-Crystal-Structures/blob/main/Final%20Presentation.pdf)

###### Note: Each of the Python files should have some examples at the end of how to run the functions and what the output looks like 

## Calculations and Plotting - No Edge Cases.ipynb:
- This file does the mismatch calculations and plotting (only plots the optimal arrangement right now) for a given set of ions
- There is an example with all of the Ag-Bi-Br combinations and their minimized total mismatches. If you want to do the same thing with other sets of ions, you can generate a csv from `GenerateAllPossibleIonSets.ipynb` and use the code I have in the last two cells of this file and just change out the variable names


## GenerateAllPossibleIonSets.ipynb:
- This will calculate all possible sets of 1+/2+/3+ or 2+/4+/vacancy ions
   - You can control if you want specific ions to be included in the sets (see comments and examples in code for this)
- Can specify if you want redox considerations or note (see comments and examples in code for this)
- Have the option to output the possible combinations/ion sets to a csv file (see comments and examples in code for this)
    - Then, you can open this csv in  `Calculations and Plotting - No Edge Cases.ipynb` and run the code for each row in the csv file (see comments and examples in code for this)

## experimental_bond_lengths.csv, updatedRedox.csv, and allCharges.csv: 
- Contain constants that are used throughout the Python files
- If you update the csvs and re-run the code, the code will automatically update with the new data
- `allCharges.csv` is probably missing some  ions because I only used the ones listed in the periodic table figure
- `updatedRedox.csv` seems to be missing a lot of the 4+ ions

## AgBiCombinations.csv:
- Contains all the possible Ag-Bi-2+ combinations (without redox considerations)
- I included this file because it is used for one of the examples in `Calculations and Plotting - No Edge Cases.ipynb`

## cr2+Combos.csv:
- A list of all possible combinations with Cr2+ 
- I believe it does not include redox potentials (but you can double check by re-running the GenerateAllPossibleIonSets.ipynb code with Cr2+)
