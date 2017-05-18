# ConGO
cs570_2017_spring_term project

## Required
[mnist.h5](https://drive.google.com/open?id=0B3kZyL62Zw6vOUJVUE94R3FjVjQ) (need to be installed & located at "data/")

## Branches
- master branch: (1)train_example: simple LSTM, (2) train_example_conv: Conv+deconv + convLSTM
- condDec branch: master/train_example_conv + conditioned decoder
- composite branch : condDec + composite decoder
- GAN branch: composite + GAN

## Weight save & load

### save하기
- train_example: weights 폴더에 저장됨
- train_example_conv: weights_conv 폴더에 저장됨

### 저장된 weight restore하기
argv[1]에 weight 파일명을 입력하는데, 확장자명을 빼야 함.

loss~.~~~~~~ (소수점 밑 6자리까지)

```bash
$ python train_example.py weights/2017-05-10_22:51:26.218343__step0__loss2839.130859
$ python train_example_conv.py weights_conv/2017-05-10_22:51:26.218343__step0__loss2839.130859
```
