# 전처리 요건
| 전처리 분야                       | 조건 |  대상                                                  | 처리                |
|----------------------------------|------|-------------------------------------------------------|---------------------|
| 결측치 처리                       | Missing Cell    oldbalanceOrg,newbalanceOrig                 | 컬럼 해당 row 삭제   |
| 불필요한 데이터 삭제  - 컬럼      | Unique가 50%넘으면  nameOrig, nameDest 컬럼                    | 해당 컬럼 삭제       |
| 불필요한 데이터 삭제  - 로우      | isFraud=1이 하나도 없는 type에 해당 하는 컬럼    isFraud 컬럼   | 해당 row 삭제        |
| 가변수화                          | int 범주형 type                                              | 컬럼 컬럼 추가       |
| 아웃 라이어 처리                  | 평균+4*표준편차 보다 큰 row  newbalanceOrig                    | 해당 row 삭제       |

# EDA 절차
* [전처리 전략](./DataScientist_Lab_EDA.pptx)

