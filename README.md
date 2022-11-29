# drop_singularity

Attention:
Project is still in early version, while the singularity image file can be created the drop environment isn't fully functional yet. Further updates coming.

This singularity defention file is created to run the detection of RNA outliers pipeline (DROP) on high performance computing clusters. The singularity image file is based on a conda environment running drop called drop_env. Further it contains a environment.yml which contains the conda environment dependencies. 

To run the file only singularity has to be installed, the container handles all the dependencies of DROP. To run the environment first build the singularity image with the build command line argument:

singularity build drop.sif conda_environment.def

When the image is build the environment can be accessed with the following command:

singularity shell drop.sif

When in the shell the drop environment can be accessed with the command conda activate drop_env.

For further information on installing and usage of singularity visit https://docs.sylabs.io/guides/3.5/user-guide/introduction.html.

For futher information on the DROP pipeline visit the following repository:
https://github.com/gagneurlab/drop

Acknowledgements:
DROP: https://www.nature.com/articles/s41596-020-00462-5
OUTRIDER: https://www.cell.com/ajhg/fulltext/S0002-9297(18)30401-4https://www.cell.com/ajhg/fulltext/S0002-9297(18)30401-4
FRASER: https://www.nature.com/articles/s41467-020-20573-7
MAE: https://www.nature.com/articles/ncomms15824
https://genomebiology.biomedcentral.com/articles/10.1186/s13059-014-0550-8



