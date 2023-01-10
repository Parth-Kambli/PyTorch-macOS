# PyTorch on mac (M1/M2)
Steps to install PyTorch on Mac with Anaconda

## Install Anaconda
[Anaconda macos link](https://www.anaconda.com/products/distribution#macos)

## Create Anaconda environment

    conda create -n <env_name> python=3.10 -y

## Activate Anaconda environment

    conda activate <env_name>
    
## Install PyTorch

    pip install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu
    
## Test the installation

    python -c "import torch; print(torch.__version__);print(torch.tensor([4,2,0], device='mps'))"
