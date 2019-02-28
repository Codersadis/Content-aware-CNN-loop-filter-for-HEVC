
## Content-Aware Convolutional Neural Network for In-loop Filtering in High Efficiency Video Coding (TIP 2019) [[pdf]](https://ieeexplore.ieee.org/document/8630681)

### Description
The experimental results reported in our paper are based on GPU hence we provide the GPU-version of our implementation. The codec with pre-trained models as well as the third-party dependencies could be found [[here]](https://drive.google.com/file/d/10hSiVS3nxYQtME34RdMdsdwcwTPE1aSg/view?usp=sharing).

### Prerequisites
- Windows 10 64-bit OS
- Microsoft Visual Studio 2013 Ultimate (Run-time library)
- CUDA 9 (both 9.1 and 9.2 are supported)
- NVIDIA GPU 
- CUDA CuDNN (Optional)

### Usage
Please unfold the .zip file after downloading. And the pre-trained caffe-models are in the trainedmodels directories. One more parameters (to identify which caffe-model to use) should be passed for codec, eg:

Encoder: 
``` bash
> TAppEncoder.exe -c encoder_AI.cfg -o rec.yuv -CaffemodelQP 37
```

Decoder:
``` bash
> TAppDecoder.exe -b str.bin -o dec.yuv --CaffemodelQP=37
```

### Citation
If you find our code helpful in your resarch or work, please cite our paper.
```
@article{jia2019content,
  title={Content-Aware Convolutional Neural Network for In-loop Filtering in High Efficiency Video Coding},
  author={Chuanmin Jia and Shiqi Wang and Xinfeng Zhang and Shanshe Wang and Jiaying Liu and Shiliang Pu and Siwei Ma}, 
  journal={IEEE Transactions on Image Processing},
  year={2019},
  publisher={IEEE}
}
```

