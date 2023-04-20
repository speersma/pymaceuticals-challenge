# pymaceuticals-challenge

This repository contains one folder. Inside the folder are one jupyter notebook, one markdown file, and a folder containing the data used in this analysis. The markdown file details the instructions for this challenge assignment. The jupyter notebook contains analyses and visualization of a dataset of mice in a study of squamous cell carcinoma treatment. That notebook has a top level summary at the beginning of the file. Details about the study and that summary has been reproduced here for ease of access. 

# Pymaceuticals Analysis

- Pymaceuticals is a company that specializes in anti-cancer medications.
- There was a **mice study**. 249 mice who had squamous cell carcinoma (SCC) tumors received drug treatment
- Tumor development was tracked & measured over 45 days.
- **Study compared performance of Capomulin to other treatment regimens**


# Summary Report

- Capomuline and Ramicane may appear to be the most effective drugs for treating squamous cell carcinoma. These drugs display the smallest final tumor volumes of all the drug regimens by at least $20 mm^3$. Both drugs seem essentially equally effective in this respect, though Ramicane has slightly lower mean and median tumor volumes than Capomuline. However, there is one In the paragraph below I discuss two potential threats to the validity of this assertion. 

    - Mouse weight and tumor volume are strongly correlated ($r = 0.842$, $p = 1e-07$). This could potentially threaten the validity of the assertion that Ramicane and Capomulin are the best performing drugs, if and only if other drug regimens have higher mouse weights in general than Ramican and Capomulin regimens. After a quick glance at the avg. mouse weight for each drug regimen, this threat seems extremely plausible. Capomulin and Ramicane have the lowest average mouse weights by apprximately 8 grams.g Thus some of the variance in the tumor volume of the mice in Capomulin and Ramicane regimens may be explained by the lower average weight of mice. However, Ramicane and Capomulin significantly decrease the size of tumors, perhaps these two drugs have a higher concentration of later timepoints with smaller weights because the tumors got smaller and therefore the mice weighed less. This is impossible though because the weight of individual mice did not change over the whole study. Thus, it seems that some of the decreased tumor size in mice treated with Capomulin and Ramicane could be due to the decreased weight of mice in these regimens, given the high positive correlation between mouse weight and tumor volume. However, it is very interesting that all the mice started at the same tumor volume (mm3). This means that at the beginning of the study the higher weights of mice in regimens other than Capomulin and Ramicane were not correlated with higher tumor volumes, since all mice had a tumor vol of 44 $mm^3$ at timepoint 0. It is only at the final tumor volume that the correlation between mouse weight and tumor volume is revealed. Perhaps something occurred during the study that produced this correlation? 

- Additionally, it is important to know what reason certain regimens have fewer timepoints. If some drug regimens have fewer timepoints because the mouse died due to their cancer, then the results are unaffected. In contrast, if some drug regimens have a concentration of mice with fewer timepoints because of some cause unrelated to their cancer progression, then those drugs' performance might be arbitrarily minimized in the results because they only have earlier timepoints, which are likely to have higher tumor volumes considering all mice started with a tumor volume of 45 grams. All that being said, the drugs **do not** differ that much in total timepoints. While Capomulin (230) and Ramicane (228) regimens have the highest number of timepoints, most of the other regimens have approximately 180 timepoints. This leads me to believe that there are enough timepoints for each drug regimen to be accurately judged by the trends in tumor volumes and the final tumor volumes.

- There are an even amount of timepoints for male and female mice. 

