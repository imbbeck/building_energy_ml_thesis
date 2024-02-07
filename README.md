# 울산시 A 공공건물의 실 데이터를 이용한 에너지 사용량 예측 모델 구현 및 성능 평가

## 파일설명

-   [hj_data_preprocessing.ipynb](#hj_data_preprocessing.ipynb)
-   [get_weather_info.ipynb](#get_weather_info.ipynb)
-   [EDA.ipynb](#EDA.ipynb)
-   [DV~~.ipynb](#DV~~.ipynb)
-   [result.ipynb](#result.ipynb)

## hj_data_preprocessing.ipynb

raw 데이터 전처리.

## get_weather_info.ipynb

해당건물은 에너지 사용량 관련 관제점만 존재해, 기상청 api를 통해 울산시의 기상 데이터를 가져옴. - 건물의 실제 환경데이터와 오차가 있어 모델 성능 하락의 요인.

## EDA.ipynb

모델 제작 전 탐색적 데이터 분석(EDA).

## DV~~.ipynb

EDA를 통해 파악된 변수와 TSM의 도메인지식 및 윤영상 박사님과의 자문를 통해 얻은 인사이트를 고려하여 건물 에너지 소비량 예측 모델을 구현하기 위한 소스 코드. <br>

-   DV : YN - 파생변수 사용 여부 <br>
-   OP : <br>
    N - 영업시간YN 고려 x 모델 <br>
    0,1 - EDA를 통해 영업시간을 09~18시로 정의하고, 각각 09~18시 데이터로 모델 제작 및 예측, 18~09시 데이터로 모델 제작 및 예측해 그 둘을 통합 <br>
-   용도별 분리YN 모델은 각 소스코드 내에서 분류하여 구현.

## result.ipynb

분리 모델 통합 및 통합된 모델들의 성능 평가.

## Conclusion

[Conclusion.docx](Conclusion.docx)
