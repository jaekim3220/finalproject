# 코드 참고

## 데이터 생성 및 활용
1. 수집 데이터 가공
2. 개발 제한 구역에 속한 행정동을 제외
3. 분석에 사용할 파생변수를 생성 후 데이터를 병합
4. 병합한 데이터를 사용해 분석을 진행

## 회귀분석

jaekim3220/jupyter/E. 확증적 데이터 분석(CDA) /04, 05, 06

### PCA
1. jaekim3220/jupyter/E. 확증적 데이터 분석(CDA)/04. 선형회귀분석/06-주성분분석(PCA).ipynb
2. jaekim3220/Semiproject3 - 과정에서 참고

- --------------------

## 군집화

### K-Means 1
https://velog.io/@nayoung5859/K-means-clustering%EC%9C%BC%EB%A1%9C-%EB%B2%88%ED%99%94%EA%B0%80-%EC%83%81%EA%B6%8C-%EC%B0%BE%EC%95%84%EB%B3%B4%EA%B8%B0

### K-Means 2
- jupyter/F. 데이터 마이닝/02. Sklearn/13-군집.ipynb

### DBSCAN
    - jaekim3220/jupyter/F. 데이터 마이닝/02. Sklearn/15-군집-DBSCAN.ipynb
    - jaekim3220/jupyter/F. 데이터 마이닝/02. Sklearn/16-군집-DBSCAN(2).ipynb

### K-Means와 DBSCAN 차이

| 특징 | DBSCAN | K-Means |
| -- | -- | -- |
| Cluster의 모양 | 데이터의 Cluster 모양이 arbitrary하게 묶이는 경우 잘 Clustering 형성 | 데이터의 Cluster 모양이 Spherical한 경우에 잘 Clustering 형성 |
| Cluster의 갯수 | 군집화 갯수를 미리 정해주지 않아도 됨(밀도 기반) | 군집화될 갯수를 미리 정해줘야함 (centroid 기반) |
| Outlier | Clustering에 포함되지 않는 Outlier를 특정할 수 있음 | 모든 데이터가 하나의 Cluster에 포함됨 |
| Initial Setting | 초기 Cluster 상태가 존재하지 않음 | 초기 Centroid 설정에 따라 결과가 많이 달라짐 |

> DBSCAN은 데이터셋 내에 밀도가 다양할 경우 밀도가 낮은 영역에서는 클러스터가 감지되지 않을 수 있고, 밀도가 높은 영역에서는 하나의 큰 클러스터로 인식될 수 있다는 단점이 존재해 자칫 입지 선정을 위한 원활한 분석이 불가할 가능성이 존재.

> DBSCAN은 ‘밀도’를 활용하여 복잡하거나 기하학적인 형태를 가진 데이터에도 클러스터링을 적용할 수 있다는 점과 밀도에 따라 자동으로 군집을 형성하는 만큼 밀집도를 필요로 하는 입지 선정에 필요하다고 판단이 가능.

### 계층적 군집(Hierarchical Clustering)
- jaekim3220/jupyter/F. 데이터 마이닝/02. Sklearn/19~24
    - jupyter/F. 데이터 마이닝/02. Sklearn/20-계층적군집(2)2_내용추가.ipynb 를 중심으로
    - sklearn, scipy의 차이를 설명
- 계층적군집.ipynb => (my.ver)
- 데이터분석(3-2.계층군집).ipynb => (정훈님.ver)
- 계층적군집따로학습.ipynb은 데이터분석(3-2.계층군집).ipynb을 내 방식데로 반복, subplots 그린거
> - 계층적군집 학습은 계층적군집.ipynb => (my.ver)처럼 한 번에 수행하는게 맞음.<br/> 한 번에 돌리되 분석할 변수가 매우 많은 경우 차원 축소를 적용 후 모델 생성 및 학습을 진행
