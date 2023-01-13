# MarineLife_ObjectDetection
# 객체인식을 통한 실시간 해양생물 인식 프로젝트
<img width="800" img height="400" src="https://user-images.githubusercontent.com/113493692/212275743-1e60b374-4cfb-4701-84a3-90125fd5b522.png">

#### 데이터셋 : [Roboflow](https://universe.roboflow.com/aqua-zwvvt/gy-aquarium)

프로젝트 기간 : 2022.08.20. ~ 2022.09.02.

---

# 1. Subject
- 모든 사람들이 해양 생물에 대한 지식이 풍부하지 않음
- 해양 생태계에 대한 다양한 정보를 제공
- 객체 인식을 통한 해양 생물 정보 제공 시스템

# 2. Dataset

<img width = '1000' img height = '400' src = 'https://user-images.githubusercontent.com/113493692/212277153-c3e44d8a-f7df-4ad6-bca3-7533a7a24e2e.png'>

Roboflow를 통한 dataset 구축

# 3. Model

- YOLOv4 모델 핸들링

<img width = '1000' img height = '520' src = 'https://user-images.githubusercontent.com/113493692/212277803-d4927733-ccc2-455f-b44a-edadea40cc22.png'>
- Anchors 핸들링
    
    default_anchor : 12,16, 19,36, 40,28, 36,75, 76,55, 72,146, 142,110, 192,243, 459,401
    afther_handling : 10,13, 16,30, 33,23, 30,61, 62,45, 59,119, 116,90, 156,198, 373,326
    
<img width = '1000' img height = '520' src = 'https://user-images.githubusercontent.com/113493692/212280371-1ecafa44-b6a3-4ed0-bc75-7af66eee14bc.png'>

- 아쿠아리움 Dataset(YOLOv5)
<img width = '1000' img height = '400' src = 'https://user-images.githubusercontent.com/113493692/212279864-dc818e56-4060-49e6-8aab-1614e17254cf.png'>

- 아쿠아리움 Dataset(YOLOv6)
<img width = '1000' img height = '100' src = 'https://user-images.githubusercontent.com/113493692/212280083-ef3205da-22c1-4f60-9b3b-ed33166a4c6d.png'>

- 상어 Dataset 추가 이유
<img width = '1000' img height = '450' src = 'https://user-images.githubusercontent.com/113493692/212280677-55e887a8-5653-402a-ac9d-64dc97e29cd8.png'>

- 아쿠아리움 + 상어 Dataset (YOLOv4) (without mosaic)
<img width = '1000' img height = '100' src = 'https://user-images.githubusercontent.com/113493692/212280928-08d21661-caaf-48e0-8f7b-033efa84c9fd.png'>

# 4. Result

- Imbalanced Data를 활용한 결과인 mAP 77%의 수치는 나쁘지 않았다고 판단
- 더욱 다양한 데이터와 Class Imbalance와 해상도 문제를 해결한다면 상용화 가능한 모델 개발 가능하다고 판단
