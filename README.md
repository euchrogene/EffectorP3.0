# This is for EuchroGene Members.

EffectorP 3.0 is a machine learning-based prediction tool designed to identify fungal effector 
proteins from secretomes, distinguishing them from non-effector secreted proteins based on specific 
physicochemical properties.

Functions:

 - Predict Fungal Effectors: Classifies secreted proteins as either effectors or non-effectors 
   using an ensemble of machine learning models.
 - Determine Localization: Distinguishes between cytoplasmic effectors (enter host cells) and 
   apoplastic effectors (remain in the extracellular space).
 - Analyze Sequence Features: Evaluates characteristics such as protein length, molecular weight, 
   net charge, and amino acid composition to inform predictions.
 - Screen High-Throughput Data: Efficiently processes large-scale secretome datasets derived from 
   fungal genomes or transcriptomes to prioritize candidates for experimental validation.

## To install, copy and paste the following commands in a Jupyter Terminal, and execute:

1. install the software:
```
wget https://github.com/euchrogene/EffectorP3.0/raw/refs/heads/main/Install_EffectorP3.0.sh
sudo bash Install_EffectorP3.0.sh
sudo rm Install_EffectorP3.0.sh
```

2. display installed software
```
EG_tools
```

4. download example protein sequence
```
wget https://github.com/euchrogene/InterProScan_EG/raw/refs/heads/main/test_prot.fa
```

5. example command line
```
EffectorP3.0 -db_path InterProScan_DB -i test_prot.fa -dp -f TSV
```

6. show help contents
```
EffectorP3.0
```

## Help contents:
```
________________________________________________________________________________________________

Tool Type: EffectorP 3.0

EffectorP 3.0 is a machine learning-based prediction tool designed to identify fungal effector 
proteins from secretomes, distinguishing them from non-effector secreted proteins based on specific 
physicochemical properties.

Functions:

 - Predict Fungal Effectors: Classifies secreted proteins as either effectors or non-effectors 
   using an ensemble of machine learning models.
 - Determine Localization: Distinguishes between cytoplasmic effectors (enter host cells) and 
   apoplastic effectors (remain in the extracellular space).
 - Analyze Sequence Features: Evaluates characteristics such as protein length, molecular weight, 
   net charge, and amino acid composition to inform predictions.
 - Screen High-Throughput Data: Efficiently processes large-scale secretome datasets derived from 
   fungal genomes or transcriptomes to prioritize candidates for experimental validation.

If you find any bugs, please email: bioinformatics@euchrogene.com

________________________________________________________________________________________________

You can run this software by modifying the following example:

EffectorP3.0 -i test_prot.fa -o Effector_results.tsv -E effector_fasta.fa -N non-effector_fasta.fa
________________________________________________________________________________________________

Usage;

# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
# EffectorP 3.0: Prediction of apoplastic and cytoplasmic effectors in fungi and oomycetes
# http://effectorp.csiro.au/
# Copyright (C) 2021-2022 Jana Sperschneider.
# Freely distributed under the GNU General Public License (GPLv3).
# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
    
Usage for EffectorP 3.0: 
python EffectorP.py [-options] -i <input_file>

where basic options are:
-f : run in fungal mode
-h : show brief help on version and usage

options directing output:
-o <f> : direct tab-delimited output table with predictions to file <f>, not stdout
-E <f> : save predicted effectors to FASTA file <f>
-N <f> : save predicted non-effectors to FASTA file <f>

# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

______________________________________________________________________________________________
```


# Citation

## EffectorP 3.0
Sperschneider J, Dodds P. EffectorP 3.0: prediction of apoplastic and cytoplasmic effectors in fungi and oomycetes. Mol Plant Microbe Interact. 2021. doi: 10.1094/MPMI-08-21-0201-R
