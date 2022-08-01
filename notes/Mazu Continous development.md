---
tags: [mazu]
title: Mazu Continous development
created: '2022-02-01T06:32:37.929Z'
modified: '2022-03-01T05:59:33.457Z'
---

# Mazu Continous development

### Creating Singleplex training data
First we need to create the submission sheet, that means we need to go through the singleguide data 

checklist
[x] download fastqs --> move to s3
[] create submission sheet 
[] Add reference sequences to submission sheet
[] Run through all samples locally
[] Build infra for remote loading from s3 for all samples
[] Create validation plots against "known" results and crispresso

lets fix this error 
*syntheseas.mazu.analysis.analyze_local_data_batch ERROR:'DataFrame' object has no attribute 'normalized_percentages'* 



what is our local folder


python -m scripts.run_analysis_CLI -d /Users/nicholas.rossi/Documents/Repos/2022/02/cleaning_mazu_dadta/clean_mazu.csv  -f /Users/nicholas.rossi/Documents/Repos/2022/02/cleaning_mazu_dadta/no_donor  -o /Users/nicholas.rossi/Documents/Repos/2022/02/cleaning_mazu_dadta/output  -p True -c True


What fraction of these are passing as is

