# Classification of agricultural pests through digital images using deep learning

Pedro Lucas de Oliveira Costa1, Thiago Matheus de Oliveira Costa 1,
Larissa Ferreira Rodrigues Moreira 1, Leandro H. F. P. Silva 1, João Fernando Mari 1*

#### Pedro Lucas de Oliveira Costa(1), Thiago Matheus de Oliveira Costa(1), Larissa Ferreira Rodrigues Moreira(1), Leandro H. F. P. Silva(1), João Fernando Mari(1)

##### (1) Instituto de Ciências Exatas e Tecnologicas - Universidade Federal de Vicosa - UFV, Rio Paranaıba, MG, Brazil

#### *{pedro.l.costa@ufv.br, larissa.f.rodrigues, joaof.mari}@ufv.br*
---

* Code for the paper published in the XIX Workshop of Computer Vision 2024 - WVC'2024.
    * wvc2024.ufv.br
---

## The development environment

* Install Anaconda from the Website https://www.anaconda.com/.

### Creating the conda environment
```
    $ conda update -n base -c defaults conda
    
    $ conda create -n env-CNNpestes-py310 python=3.10
    $ conda activate env-CNNpestes-py310

    $ conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
    $ conda install chardet
    $ pip install notebook
    $ pip install matplotlib
    $ pip install scikit-image
    $ pip install scikit-learn
    $ pip install pandas
    $ pip install seaborn
    $ pip install ipywidgets
    $ pip install ipympl
    $ pip install graphviz
    $ pip install opencv-python
    $ pip install albumentations
    $ pip install timm

```

### Save environment

```
    $ conda env export > env-CNNpestes-py310.yml
```

### Load enviroment from yml file

```
    $ conda env create -f env-CNNpestes-py310.yml 
```

## Converting ipynb to py
---

```
    $ jupyter nbconvert CNNPestes.ipynb --to python
```


## Executing the experiments

### Hyperparameter experiments

```
    $ nohup python grid-search.py --arch alexnet --optimizer Adam &
    $ nohup python grid-search.py --arch efficientnet_b4 --optimizer Adam &
    $ nohup python grid-search.py --arch mobilenet_v3 --optimizer Adam &
    $ nohup python grid-search.py --arch resnet50 --optimizer Adam &
```

* Pick up the best hyperparameter values

### Main experiments

* Run each experiment throug CNNpestes.py, or...
* Set the experiments thall will run in the train_test_batch.py

```
    $ nohup python train_test_batch.py
```

## Utilities:
---

* Memória da GPU não libera, mesmo nvidia-smi não mostrando nenhum processo:
    * https://stackoverflow.com/a/46597252

```
fuser -v /dev/nvidia*
                     USER        PID ACCESS COMMAND
/dev/nvidia0:        joao      44525 F...m python
/dev/nvidiactl:      joao      44525 F...m python
/dev/nvidia-uvm:     joao      44525 F...m python

kill -9 44525
```

* List Python processes
```
    $ ps -ef | grep python
```
