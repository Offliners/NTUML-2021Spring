![cover](https://github.com/Offliners/OFF/blob/main/cover.png)

Course Syllabus : [Link](https://speech.ee.ntu.edu.tw/~hylee/ml/2021-spring.html)

## Outline
|#|Homework|Slide|Code|Public score|Private Score|Score|
|-|-|-|-|-|-|-|
|0|Colab Tutorial|[Link](HW0/Google_Colab_Tutorial.pdf)|[Colab Tutorial](HW0/Colab_Tutorial.ipynb)|x|x|x|
|0|Pytorch Tutorial|[Link](HW0/Pytorch_Tutorial_1.pdf) [Link](HW0/Pytorch_Tutorial_2.pdf)|[Pytorch Tutorial](HW0/Pytorch_Tutorial.ipynb)|x|x|x|
|1|Regression|[Link](HW1/HW01.pdf)|[COVID-19 Cases Prediction](HW1/homework1.ipynb)|`0.86928`|`0.92417`|9|
|2|Classification|[Link](HW2/HW02.pdf)|[Phoneme Classification](HW2/homework2_1.ipynb)|`0.75171`|`0.74957`|6|
|2|Linear Algebra|[Link](HW2/HW02.pdf)|[Hessian Matrix](HW2/homework2_2.ipynb)|x|x|2|
|3|CNN|[Link](HW3/HW03.pdf)|[Image Classification](HW3/homework3.ipynb)|`0.77956`|`0.77166`|8|
|4|Self-Attention|[Link](HW4/HW04.pdf)|[Phoneme classification](HW4/homework4.ipynb)|`0.95928`|`0.95833`|10+0.5([report](HW4/hw4_report.pdf))|
|5|Transformer|[Link](HW5/HW05.pdf)|[Machine Translation](HW5/homework5.ipynb)|`26.44`|`25.54`|8|
|6|GAN|[Link](HW6/HW06.pdf)|[Anime Face Generation](HW6/homework6.ipynb)|`0.710`, `7716.47`|`0.710`, `7716.47`|10+0.5([report](HW6/hw6_report.pdf))|
|7|BERT|[Link](HW7/HW07.pdf)|[Question Answering](HW7/homework7.ipynb)|`0.81178`|`0.81833`|9|
|8|Anomaly Detection|[Link](HW8/HW08.pdf)|[Anomaly Detection](HW8/homework8.ipynb)|`0.89049`|`0.88126`|10+0.5([report](HW8/hw8_report.pdf))|
|9|Explainable AI|[Link](HW9/HW09.pdf)|[Explainable AI](HW9/homework9.ipynb)|x|x|8.4|
|10|Attack|[Link](HW10/HW10.pdf)|[Adversarial Attack](HW10/homework10.ipynb)|`0.000`|`0.010`|10+0.5([report](HW10/hw10_report.pdf))|
|11|Adaptation|[Link](HW11/HW11.pdf)|[Domain Adaptation](HW11/homework11.ipynb)|`0.81598`|`0.81690`|10+0.5([report](HW11/hw11_report.pdf))|
|12|RL|[Link](HW12/HW12.pdf)|[Reinforcement Learning](HW12/homework12.ipynb)|`280`|`280`|10+0.5([report](HW12/hw12_report.pdf))|
|13|Compression|[Link](HW13/HW13.pdf)|[Food Classification](HW13/homework13.ipynb)|`0.80167`|`0.81350`|9.5|
|14|Life-Long Learning|[Link](HW14/HW14.pdf)|[Permuted MNIST](HW14/homework14.ipynb)|x|x|8.8|
|15|Meta Learning|[Link](HW15/HW15.pdf)|[Few-shot image classification](HW15/homework15.ipynb)|x|x|9.2|

## Note
|Week|Topic|Link|Week|Topic|Link|
|-|-|-|-|-|-|
|1|Introduction of ML/DL|[Link](https://offliners.github.io/post/ntuml-week1/)|8|BERT|[Link](https://offliners.github.io/post/ntuml-week8/)|
|2|General Guidance|[Link](https://offliners.github.io/post/ntuml-week2-1/)|9|Midexam|x|
|2|When Gradient Is Small: Local Minimum and Saddle Point|[Link](https://offliners.github.io/post/ntuml-week2-2/)|10|Auto-Encoder|[Link](https://offliners.github.io/post/ntuml-week10/)|
|2|Tips for Training: Batch and Momentum|[Link](https://offliners.github.io/post/ntuml-week2-3/)|11|Adversarial Attack|[Link](https://offliners.github.io/post/ntuml-week11/)|
|3|Tips for Training: Adaptive Learning Rate|[Link](https://offliners.github.io/post/ntuml-week3-1/)|12|Machine Learning and Privacy|`TBD`|
|3|Loss Function: Classification|[Link](https://offliners.github.io/post/ntuml-week3-2/)|13|Explainable AI|[Link](https://offliners.github.io/post/ntuml-week13/)|
|3|CNN|[Link](https://offliners.github.io/post/ntuml-week3-3/)|14|Domain Adaptation|[Link](https://offliners.github.io/post/ntuml-week14/)|
|4|PAC Learning|`TBD`|15|Quantum Machine Learning|`TBD`|
|5|Self-Attention|[Link](https://offliners.github.io/post/ntuml-week5-1/)|16|Reinforcement Learning|[Link](https://offliners.github.io/post/ntuml-week16/)|
|5|Normalization|[Link](https://offliners.github.io/post/ntuml-week5-2/)|17|Life-long Learning|[Link](https://offliners.github.io/post/ntuml-week17-1/)|
|6|Qingming Festival|x|17|Network Compression|[Link](https://offliners.github.io/post/ntuml-week17-2/)|
|7|Transformer|[Link](https://offliners.github.io/post/ntuml-week7-1/)|18|Meta Learning|[Link](https://offliners.github.io/post/ntuml-week18/)|
|7|GAN|[Link](https://offliners.github.io/post/ntuml-week7-2/)|-|-|-|

## Useful Tips
### Prevent Google Colab from disconnecting (valid utill 2021/06/25)
Press `F12`，and enter this code in console，then press `enter`
```javascript
function ClickConnect(){
  console.log("Connnect Clicked - Start"); 
  document.querySelector("#top-toolbar > colab-connect-button").shadowRoot.querySelector("#connect").click();
  console.log("Connnect Clicked - End"); 
};
setInterval(ClickConnect, 60000)
```

### Auto save output file on Google Colab
insert code cell at the bottom
```python
from google.colab import files
files.download("output_file.csv")  # "output_file.csv" must be your output file name
```

### Display information of GPU of Google Colab
insert code cell to check which GPU is assigned
```shell
!nvidia-smi
```
### "Sorry, something went wrong. Reload?" when viewing *.ipynb on Github
Copy the URL to https://nbviewer.jupyter.org/

## Student Source
<p align="center">
<img src="https://github.com/Offliners/OFF/blob/main/StudentSource.jpg" alt="Student Source">
</p>

## Homework Participation
<p align="center">
<img src="https://github.com/Offliners/OFF/blob/main/HomeworkParticipation.JPG" alt="Class Participation">
</p>

## My Performance
<p align="center">
<img src="https://github.com/Offliners/OFFML/blob/main/myPerformance.jpg" alt="My Performance">
</p>

## Reference
* TA's github : https://github.com/ga642381/ML2021-Spring
* Pytorch documentation : https://pytorch.org/docs/stable/index.html
