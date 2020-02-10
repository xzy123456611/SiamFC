# Pytorch implementation of SiamFC

## Run demo
```bash

mkdir models

```

## Training
Download ILSVRC2015-VID 

```bash
cd SiamFC

mkdir models

# using 12 threads should take an hour
python bin/create_dataset.py 

# ILSVRC2015_VID_CURATION and ILSVRC2015_VID_CURATION.lmdb should be in the same directory
# the ILSVRC2015_VID_CURATION.lmdb should be about 34G or so
python bin/create_lmdb.py -

# training should take about 1.5~2hrs on a Titan Xp GPU with 30 epochs
python bin/train_siamfc.py 
```
## Benchmark results
#### OTB100

| Tracker 			    		 | AUC             |
| ---------------------------------------------  | --------------- |
| SiamFC(trained from scratch)      		 | 0.5xx           |

## Note
We use SGD without momentum, weight decay setting 0, detailed setting can be found in config.py
Training is unstable
```bash
Epoch 1 AUC:
Epoch 2 AUC:

Epoch n AUC:
```
## Reference
Bertinetto, Luca and Valmadre, Jack and Henriques, Joo F and Vedaldi, Andrea and Torr, Philip H S
		Fully-Convolutional Siamese Networks for Object Tracking
		In ECCV 2016 workshops
