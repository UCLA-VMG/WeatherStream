# WeatherStream: Light Transport Automation of Single Image Deweathering (CVPR'23)
Howard Zhang<sup>1*</sup>, Yunhao Ba<sup>1*</sup>, Ethan Yang<sup>1</sup>, Varan Mehra<sup>1</sup>, Blake Gella<sup>1</sup>, Akira Suzuki<sup>1</sup>, Arnold Pfahnl<sup>1</sup>, Chethan Chinder Chandrappa<sup>1</sup>, Alex Wong<sup>2</sup>, Achuta Kadambi<sup>1</sup>

University of California, Los Angeles<sup>1</sup>, Yale University<sup>2</sup>

## Project Webpage
[https://visual.ee.ucla.edu/wstream.htm/](http://visual.ee.ucla.edu/wstream.htm/)

## Abstract
Today single image deweathering is arguably more sensitive to the dataset type, rather than the model. We introduce WeatherStream, an automatic pipeline capturing all real-world weather effects (rain, snow, and rain fog degradations), along with their clean image pairs. Previous state-of-the-art methods that have attempted the all-weather removal task train on synthetic pairs, and are thus limited by the Sim2Real domain gap. Recent work has attempted to manually collect time multiplexed pairs, but the use of human labor limits the scale of such a dataset. We introduce a pipeline that uses the power of light-transport physics and a model trained on a small, initial seed dataset to reject approximately 99.6% of unwanted scenes. The pipeline is able to generalize to new scenes and degradations that can, in turn, be used to train existing models just like fully human-labeled data. Training on a dataset collected through this procedure leads to significant improvements on multiple existing weather removal methods on a carefully human-collected test set of real-world weather effects.

## Citation

```
@inproceedings{zhang2023weatherstream,
  title={WeatherStream: Light Transport Automation of Single Image Deweathering},
  author={Zhang, Howard and Ba, Yunhao and Yang, Ethan and Mehra, Varan and Gella, Blake and Suzuki, Akira and Pfahnl, Arnold and Chandrappa, Chethan Chinder and Wong, Alex and Kadambi, Achuta},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  year={2023}
}
```

## Dataset
The dataset can be found [here](https://drive.google.com/drive/folders/12Z9rBSTs0PPNHLieyU2vnCTzR6fOFLrT).

## Model
Initial seed model uses GT-RAIN [here](https://github.com/UCLA-VMG/GT-RAIN).

## Requirements
All code was tested on Google Colab with the following:

- Ubuntu 18.04.6
- CUDA 11.2
- Python 3.7.13
- OpenCV-Python 4.6.0
- PyTorch 1.12.1
- scikit-image 0.18.3
## Setup
Download initial seed model from link above. Set the model and pipeline parameters. Set the folder name in the main pipeline loop. Make sure directory structure follows code comment.  

## Disclaimer
Please only use the code and dataset for research purposes.

## Contact
Yunhao Ba</br>
UCLA, Electrical and Computer Engineering Department</br>
yhba@ucla.edu

Howard Zhang</br>
UCLA, Electrical and Computer Engineering Department</br>
hwdz15508@g.ucla.edu
