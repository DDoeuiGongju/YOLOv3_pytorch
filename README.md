# YOLOv3 with pytorch
"YOLOv3: An Incremental Improvement" paper implementation  
※ https://arxiv.org/abs/1804.02767

### YOLOv3 model구현한 순서
1. darknet-53 구조 구현
2. YOLOv3 구조 구현
3. YOLOv3 detection 구현
    - build target 구현
    - bbox_wh_iou 구현: 박스의 모양에 관한 iou
    - 손실 계산
4. NMS 구현
    - bbox_iou 구현: 박스의 위치에 대한 iou
5. dataset 준비
    - https://drive.google.com/file/d/1wJn0GOGcWpHwe60tN3lP63cb28lEqemJ/view?usp=sharing 에서 yolov3.zip파일 다운
    - 자세한 내용 setup_coco_dataset.sh 파일의 주석 참고
    - 리눅스 터미널에서 아래의 명령어 실행(본인은 cygwin 사용)
    - bash setup_coco_dataset.sh
        - bash 했을 때 잘 안되면 터미널에서 파일 안의 코드를 한줄 한줄 실행한다. 
