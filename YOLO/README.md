# Capstone_Design
<div align="center">
  <p>
    <a align="center" href="https://github.com/Chaelsy-kim/Capstone_Design" target="_blank">
      <img width="850" height="200" src="https://user-images.githubusercontent.com/51262434/201677642-1f8273d5-15f6-4980-92a4-7fcb51e84475.png"></a>
  </p>

  <div>
    <a href="https://colab.research.google.com/drive/1ucTPBdeuFCH8yVHlZkP-Gl2MnlZ_PpzO?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
  </div>

  <br>
  <p>
    금속활자판본인지 목재활자판본인지 구별하는 모델입니다. <a href="https://github.com/ultralytics/yolov5">YOLO 모델</a>을 전이학습하여 높은 정확도의 모델을 만들었습니다.
    <br><br>
  </p>
</div>

* * *

# 데이터전처리
## PREPROCESSING

- Auto-Orient: Applied
- Resize: Stretch to 640x640
- Auto-Adjust Contrast: Using Contrast Stretching
- Grayscale: Applied

## AUGMENTATIONS

- Outputs per training example: 3
- Saturation: Between -25% and +25%
- Brightness: Between -20% and +20%
- Exposure: Between -10% and +10%
- Blur: Up to 1px
- Noise: Up to 5% of pixels

## BALANCING
- data of metal type book: x2

# Test 결과
## 금속활자
![image](https://user-images.githubusercontent.com/51262434/201683891-d0c9816e-9b97-4105-9718-c4eededf8220.png)
12개 중 12개 정답
## 목판
![image](https://user-images.githubusercontent.com/51262434/201686748-2ae9a97a-df11-4b73-b088-3b8dffd4763f.png)
8개 중 7개 정답
