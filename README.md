## Installation
* Install dependencies. We use python 3.7 and pytorch >= 1.2.0
```
clone후 conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=10.0 -c pytorch로 torch 및 torchvision 설치 후 
pip install -r requirements.txt로 관련 패키지를 설치하신 뒤
cd src/lib/models/networks/DCNv2_new sh make.sh 에서 DCN Network 빌드하시고 아래의 링크를 통해 all_hrnet_v2_w18.pth를 받아 상위폴더에 models 폴더 만들어서
fairmot/models 위치에 해당 .pth파일을 넣어 주시면 됩니다.
```
HRNetV2_W18: [[Google]](https://drive.google.com/open?id=182EHCOSzVVopvAqAXN5o6XHX4PEyLjZT) [[Baidu, code: z4ft]](https://pan.baidu.com/s/1h1qwn8dyJmKj_nZi5H3NAQ).
After downloading, you should put the baseline model in the following structure:
```
${FAIRMOT_ROOT}
   └——————models
           └——————all_hrnet_v2_w18.pth
           └——————...
```

## Demo
python demo.py를 이용하면 WebCam에서 동작하는 데모 파일을 실행하실 수 있습니다.
