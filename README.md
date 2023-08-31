# LS-SOD
Official Implementation of "Low-Light Salient Object Detection Meets the Small Size"
- Since our paper is still under review, we will release our code and dataset once the paper is accepted. Thanks for your understanding.

## Prerequisites
- [Python 3.5](https://www.python.org/)
- [Pytorch 1.3.1](http://pytorch.org/)
- [OpenCV 4.4.0.42](https://opencv.org/)
- [Numpy 1.16.2](https://numpy.org/)
- [TensorboardX 2.1](https://github.com/lanpa/tensorboardX)
- [Apex](https://github.com/NVIDIA/apex)

## Download dataset
Download the following dataset and unzip them into `data` folder
We conduct experiments on our proposed NTI dataset and a widely used dataset, DUTS-TE.
- [DUTS](http://saliencydetection.net/duts/)
- NTI dataset will be available upon acceptance of our manuscript.

## Training
Training code will be available upon acceptance of our manuscript.

## Testing
Testing code will be available upon acceptance of our manuscript.

## Evaluation
```shell
cd eval
matlab
main
```

## Saliency maps
We provide prediction results of our proposed IEDNet model based on different backbones through SI, on the DUT-TE dataset.
| Model         | Backbone           | Test Set       |  Predictions  |
|---------------|----------------|-----------------|------------|
| IEDNet | ResNet | DUT-TE | [DUT-TE](https://drive.google.com/file/d/1d5zSqUti2ubvhDOMUSZoNAP3a5MG4Fv_/view?usp=sharing) 
| IEDNet | Res2Net | DUT-TE | [DUT-TE](https://drive.google.com/file/d/13Fp-c3mHX8sOw18NRyLTyUxvuzh6Oaj2/view?usp=sharing) 
| IEDNet |  PVTV2-1K | DUT-TE | [DUT-TE](https://drive.google.com/file/d/1fggNZLdVLe3YKK3YiqS8hh3HnlN_cNHe/view?usp=sharing) 

Meanwhile, we provide the Mask2Former model trained on synthetic COCO (synthesized by our SI strategy).

| Model         | Backbone           | Train set       | Box AP | Config | CKPT |
|---------------|----------------|-----------------|------------|-----------------|------------|------------|
| Mask2Former | ResNet50 | Syn COCO | 38.9 | [Config](https://drive.google.com/file/d/1pSHm0h84Qgj2gVD1FgDGQvfi4PxdoAKm/view?usp=sharing) |[CKPT](https://drive.google.com/file/d/1Hr71EfT_vUMpLkFqampevLbljBcNnsms/view?usp=sharing) 

- If you have any questions, please get in touch with wangshiqin@wust.edu.cn





