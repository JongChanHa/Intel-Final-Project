Project name
실시간 표정에 따른 배경 색 제어
Requirement
* 10th generation Intel® CoreTM processor onwards
* At least 32GB RAM
* python3.9.13
Git
[openvino] https://github.com/openvinotoolkit/open_model_zoo
[project] https://github.com/JongChanHa/Intel_AI_project01

Prerequite
작업 폴더 생성
mkdir work
cd work
python 가상환경 생성
python -m venv openvino_env
openvino_env\Srcipts\activate
git clone
git clone https://github.com/openvinotoolkit/open_model_zoo.git
git clone https://github.com/JongChanHa/Intel_AI_project01
pip install
cd open_model_zoo
python -m pip install -U pip
pip install -r .\demos\common\python\requirements.txt
pip install openvino
cd ..
폴더 구조
├── open_model_zoo
├── Intel_AI_project01
└── openvino_env
Steps to build
pretrained model download&converter
cd Intel_AI_project01
type models.lst

omz_downloader --list models.lst
omz_converter --list models.lst
Steps to run
activate env (이미 켜져 있다면 건너뛰기)
openvino_env\Srcipts\activate
demo실행
python demo.py
결과 동영상을 저장하고 싶을때
python demo.py --o output.avi
Output
output.gif

Appendix
(참고 자료 및 알아두어야할 사항들 기술)
