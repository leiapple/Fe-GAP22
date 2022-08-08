# Fe-GAP22

Fe-GAP22 is a Gaussian approximation potential (GAP) by extending a DFT database for ferromagnetic bcc iron (https://archive.materialscloud.org/record/2017.0006/v2) to include highly distorted primitive bcc cells and surface separation, along with small crack-tip configurations that are identified by means of a fully automated active learning workflow. 

The repository includes DFT database, potential file and training commands of Fe-GAP22.

## QUIP training commands (train.in)
Three descriptors are used to encode the local atomic environment, i.e., one distance-based 2-body interaction and two many-body turbo-SOAP descriptors. Two turbo-SOAP descriptors are used to describe the inner and outer atomic environment within the cutoff radius of 3.5 Å and 5 Å, respectively. Dot product kernel is used for both turbo-SOAP descriptors, and the CUR matrix decomposition procedure is applied to find the optimal representative local atomic environments. The cutoff smoothing distance is set to 1 Å. The number of radial and angular basis for turbo-SOAP are set to 8.

## GAP potential file (GAP_model)

## New DFT database (New_DBs)