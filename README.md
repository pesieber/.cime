# .cime
CIME configuration files for running CESM/CTSM on pizdaint: has to be at $HOME/.cime   
In config_compilers.xml, manually replace the user-specific path to the oasis installation by your own path

Install oasis:   
spack install oasis@master%gcc@9.3.0 fflags="-ffree-line-length-512"

Identify  location of library links to be put into config_compilers.xml:   
spack location -i oasis%gcc
