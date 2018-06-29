# NIRSpec Target Acquisition (TA)

## This repo

The code in this repo is meant to be an exact reproduction of the OSS code so that we get
exactly the same TA images as OSS. 

-> All scripts are witten in Python 3. 


## Get started


- Prepare to run the ```OSScandidatestars.py``` script. To do this, you make sure that 
you have the following directory structure. Create the directory where you will place
everything under:
```bash
mkdir OSS_NRS_TA
```


- Clone or fork the repo. Go into the new directory ```OSS_NRS_TA```. To clone the repo, 
at the top of this page copy the ulr that appears in the "Clone or download" green 
button, and then type:
```bash
git clone the_ulr_you_copied
```


- This is the directory structure for the code to run:
```
OSS_NRS_TA
   |____src
         |________OSS_candidate_stars
         |________SIAF_files
         |________all scripts.py, readme, licence, and code of conduct files
   
   |____sim_scenes
           |___Scene_1_AB23
           |___Scene_2_AB1823
   
   |____results_OSScandidatestars
           |_____text files where the OSScandidatestars.py will dump results 
```  

- Get the data to run the script from central store. Make sure you are in the 
```OSS_NRS_TA``` directory, and then copy the files: 
with:
```bash
cp -rf /grp/jwst/wit4/nirspec/nirspec_TA/sim_scenes .
```


- To run the code do the follwing in a terminal, under the ```src``` directory:
```bash
python OSScandidatestars.py
```
If all went well you should have 23 text files in the ```results_OSScandidatestars``` 
directory. You can compare with what is in the directory with the same name in central
store.
