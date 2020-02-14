# Pytorch implementation of SiamFC

## Run demo
```bash

```

## Training

```bash
#(1) Create dataset using 12 threads should take an hour
#(2) Dataset ILSVRC2015_VID_CURATION and ILSVRC2015_VID_CURATION.lmdb should be in the same directory
#(3) The ILSVRC2015_VID_CURATION.lmdb should be about 34G or so
#(4) Training should take about 1.5~2hrs on a Titan Xp GPU with 30 epochs
```
## Testing

```bash

```
## Benchmark results
#### OTB100

|         Tracker        |       AUC       |
| ---------------------- | --------------- |
|         SiamFC         |      0.5xx      |


## Reference
```bash
Bertinetto, Luca and Valmadre, Jack and Henriques, Joo F and Vedaldi, Andrea and Torr, Philip H S
		Fully-Convolutional Siamese Networks for Object Tracking
		In ECCV 2016 workshops
```
