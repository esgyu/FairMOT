## Installation
* Install dependencies. We use python 3.7 and pytorch >= 1.2.0
```
1. clone후 conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=10.0 -c pytorch로 torch 및 torchvision 설치  

2. pip install -r requirements.txt로 관련 패키지 설치  

3. src/lib/models/networks/DCNv2_new sh make.sh 실행  

4. 아래 링크에 있는 all_hrnet_v2_w18.pth 파일 다운로드 후 models 폴더 새로 만들어서 fairmot/models 위치에 해당 .pth파일을 넣어 주시면 됩니다.  
```
HRNetV2_W18: [[Google]](https://drive.google.com/open?id=182EHCOSzVVopvAqAXN5o6XHX4PEyLjZT) [[Baidu, code: z4ft]](https://pan.baidu.com/s/1h1qwn8dyJmKj_nZi5H3NAQ).  
HRNetV2 ImageNet pretrained model: [HRNetV2-W18 official](https://1drv.ms/u/s!Aus8VCZ_C_33cMkPimlmClRvmpw)  
After downloading, you should put the baseline model in the following structure:

```
${FAIRMOT_ROOT}
   └——————models
           └——————all_hrnet_v2_w18.pth
           └——————...
```

## Demo
python demo.py를 이용하면 WebCam에서 동작하는 데모 파일을 실행하실 수 있습니다.  
