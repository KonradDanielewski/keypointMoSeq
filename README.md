# Keypoint MoSeq

Implementation of [keypoint-SLDS](https://www.overleaf.com/read/rkpnxchbdrrb) aproach for unsupervised behavior discovery. Check out our [colab notebook](https://colab.research.google.com/github/calebweinreb/keypointMoSeq/blob/user_friendly_pipeline/examples/keypointMoSeq_demo_colab.ipynb) for a tutorial. 

## Installation

1. If you plan to use a GPU (recommended), install the appropriate driver and CUDA version. CUDA ≥11.1 and cuDNN ≥8.2 are required. [This section of the DeepLabCut docs](https://deeplabcut.github.io/DeepLabCut/docs/installation.html#gpu-support) may be helpful.


2. Install [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html). Create and activate an environment called `keypoint_moseq` with python 3.9:
```
conda create -n keypoint_moseq python=3.9
conda activate keypoint_moseq

# Include the following line if installing on Windows
# conda install -c conda-forge pytables
```

3. Install jax
```
# MacOS and Linux users (CPU)
pip install "jax[cpu]"

# MacOS and Linux users (GPU)
pip install "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html

# Windows users (CPU)
pip install jax https://whls.blob.core.windows.net/unstable/cpu/jaxlib-0.3.22-cp39-cp39-win_amd64.whl

# Windows users (GPU)
pip install jax https://whls.blob.core.windows.net/unstable/cuda111/jaxlib-0.3.22+cuda11.cudnn82-cp39-none-win_amd64.whl
```

4. Clone or download the this github repo and pip install:
```
git clone https://github.com/calebweinreb/keypointMoSeq.git
pip install keypoint_moseq
```

5. Make the new environment accessible in jupyter 
```
python -m ipykernel install --user --name=keypoint_moseq
```
