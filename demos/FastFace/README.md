# BigDL-Nano Training and Inference Demo

This demo shows how to use BigDL-Nano to acclerate the model training and inference in a PyTorch Lightning based application.

The link to the original application we used in this demo is at: https://github.com/borhanMorphy/fastface.

Corresponding FDDB dataset link we used in this demo is at: http://vis-www.cs.umass.edu/fddb/.

With just a few lines of change in code, you can get 3x times of speed up in training and 2x times of speed up in inference.

## Training using BigDL-Nano
The below animation shows how the user can easily enable training using BigDL-Nano with just one line of change.
![Training demo](data/nano_training.gif)

## Inference and Quantization using BigDL-Nano
The below animation shows how the user can easily enable acceleration and quantization using BigDL-Nano with just a couple of lines of code.
![Inference demo](data/nano_inference.gif)

## How to Run the Demos

### Prepare environment

We recommend you to use Anaconda to prepare the environment. 

If you already have a nano environment, skip this step.

```
conda create -n nano python=3.7  # "nano" is conda environment name, you can use any name you like.
conda activate nano
pip install --pre bigdl-nano[pytorch]
pip install setuptools==58.0.4
pip install protobuf==3.20.1
source bigdl-nano-init
```

Next, you need to install the corresponding dependence library of face recognition through PyPl:

```
pip install fastface==0.1.3
```

If you want to experience inference pipeline acceleration, you need to install these dependence libraries through PyPl:

```
pip install neural_compressor
pip install openvino-dev
pip install onnx==1.9.0 onnxruntime==1.10.0 onnxruntime-extensions
pip install numpy --upgrade
```


### Start Jupyter
```
$jupyter notebook
```
open the notebook in a browser.

Note that the environment preparation needs to be done before the juypter kernal started. Or some of the optimziations may not take effect.
