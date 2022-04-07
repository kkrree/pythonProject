62p까지 개념

- 오존량 예측 63
- 붓꽃 품종 분류 71
- 트리 모형의 교차검증 78
- 트리 모형의 교차검증2 81 -load iris
- 와인품질 분류 86
- 타이타닉호 생존자 분류 93 -load dataset
- 신용카드 사기 거래 분류 102 -kaggle data(X)
- cancer 데이터 분류 109 -load breast cancer
----------------------------------------

#### 의사결정 나무(Decision Tree)
1. 의사결정나무 모형
    1. 일련의 독립변수들을 활용하여 분류를 하거나 예측을 수행하는 기법
    2. 최종 결과물이 '일련의 규칙들'로 표현됨
    3. Decision Trees 또는 Trees라고 불림

2. 의사결정나무의 2가지 기본 아이디어
    1. 반복전 분할(Recursive partitioning)
        1. 레코드들을 두 부분으로 반복해서 잘라 세분된 영역 내의 동질성이 최대가 되도록 함(2진분할)
        2. 계속 잘라나가다 보면 모든 학습용 데이터를 100%정확하게 분류해 낼 수 있을 만큼 세분화해 나갈 수 있음
    2. 분류나무의 가지치기(Pruning the tree)
        1. 반복적 분할을 반복하다 보면 과적합화는 피할 수 없이 나타나게 됨
        2. 과적합화를 피하기 위해 불필요한 가지(정보 제공이 적은 가지)를 제거함으로써 나무를 단순화하는 작업이 이루어지게 됨
![treesEX](https://media.springernature.com/lw785/springer-static/image/prt%3A978-1-4899-7687-1%2F4/MediaObjects/978-1-4899-7687-1_4_Part_Fig1-66_HTML.gif)
> 출처 https://link.springer.com/referenceworkentry/10.1007/978-1-4899-7687-1_66
3. 단점 : 과적합화 문제
![overfit](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_OoUfSv7AsYBwzg6wllenoUXAOI17o3DExw&usqp=CAU)
> 출처 https://vitalflux.com/overfitting-underfitting-concepts-interview-questions/
    1. 과적합화의 해소 방법 
        1. 가지치기 : 적당한 수준에서 나무의 성장을 중단시킴
        2. 랜덤 포레스트