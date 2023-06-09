
# INSTALL

## Install miniconda
See https://conda.io/projects/conda/en/latest/user-guide/install/index.html

## Install git
See https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Install docker
See https://docs.docker.com/engine/install/

## Install singurality
https://docs.sylabs.io/guides/3.0/user-guide/quick_start.html#quick-installation-steps

## Install FreeSurfer
https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall

## Install R
https://cran.r-project.org/bin/linux/ubuntu/

## Install AFNI
https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/background_install/install_instructs/index.html

## Install FSL
https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation  

## Download scilpy git repositories
```
cd
git clone https://github.com/scilus/scilpy.git
```

## Install scilpy and antspyx in conda environment
```
conda create -n tractflow python=3.10 pip hdf5=1.12 cython numpy psutil mkl -c anaconda
conda activate tractflow
cd ~/scilpy
pip install -e .
pip install antspyx
```

## Download nextflow
```
cd ~/bin
wget https://github.com/nextflow-io/nextflow/releases/download/v21.10.6/nextflow && chmod +x nextflow
rm -rf ~/.nextflow
sudo apt install default-jre
```

## Download TractoFlow and freewater_flow
```
nextflow pull scilus/tractoflow
cd
git clone https://github.com/scilus/freewater_flow
docker pull scilus/scilus:1.4.2
```

## Install c3d and connectome workbench for converting ANTs warp to FSL
Download c3d-1.0.0-Linux-x86_64.tar.gz from http://www.nitrc.org/frs/downloadlink.php/7073 into ~/Downloads  
```
cd
tar zxvf Dwonload/c3d-1.0.0-Linux-x86_64.tar.gz
cd bin
ln -sf ~/c3d-1.0.0-Linux-x86_64/c3d_affine_tool ./

sudo apt install connectome-workbench
```

## Install TractFlowProc scripts
```
cd
git clone https://github.com/mmisaki/TractFlowProc
```
