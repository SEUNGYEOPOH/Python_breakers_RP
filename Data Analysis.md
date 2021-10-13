 Data Analysis
 ======================

# 1. Data Analysis?
- Data Analysis : 데이터 분석은 인사이트 도출을 위해 알고리즘과 수학적 처리과정을 적용시켜 해당 정보에 대한 결론 도출과 패턴을 찾기 위한 목적으로 데이터를 다루는 과학.
<br>쉽게 말해 데이터를 정리, 변환하여 의사결정에 사용하기 위한 일련의 과정을 말한다. 데이터 분석은 효율적이고 과학적인 의사결정을 위해 다양한 분야에서 사용한다.

****
# 2. Data Analysis Process
## 2.1. 데이터 분석 과정
- 데이터 분석 과정은 다음과 같은 4단계를 거친다.

      1. Exploratory Data Analysis
      2. Data Preprocessing
      3. Feature Engineering
      4. Modeling
      5. 
### 2.1.1. Exploratory Data Analysis
- 탐색적 데이터 분석은 데이터를 가지고 유연하게 데이터를 탐색하고 데이터의 특징과 구조로부터 얻은 정보를 시각화하는 분석방법이다. 탐색적 데이터 분석은 본격적인 모델링을 시작하기 전 선행되어야한다.

- Exploratory Data Analysis   
    1. 문제 정의
    2. 시각화 & 변수탐색
    3. 결측치, 이상치 탐지 
### 2.1.2. Data Preprocessing
- 데이터 전처리는 데이터 분석 과정의 대부분을 차지할 정도로 굉장히 중요한 작업이다. Data set은 보통 바로 분석이 불가능하다.(Messy 하기 때문) 분석이 가능한 상태로 만드는 것이 데이터 전처리이다. 

- Data Preprocessing   
    1. 적절한 데이터 처리
    2. 정규화
    3. 교차검증 설정 
### 2.1.3. Feature Engineering
- Feature Engineering은 데이터에 대한 도메인 지식을 활용하여 특징(Feature)를 만들어내는 과정이다. 모델을 위한 데이터 테이블의 컬럼(특징)을 생성하거나 선택하는 작업을 의미한다. Feature Engineering은 모델 성능에 미치는 영향이 크기 때문에 굉장히 중요한 단계이며, 전문성과 시간과 비용이 많이 드는 작업이다.

- Feature Engineering  
    1. 변수 생성
    2. 자원 축소
    4. 특징 추출 
### 2.1.4. Modeling
- dd

- Modeling 
    1. 예측 모델링
    2. 분류 모델링
    3. 결과 해석 
 # 관련 라이브러리
 ## 1.1. Pandas
 - Pandas는 데이터 조작 및 분석을 위해 Python 프로그래밍 언어로 작성된 소프트웨어 라이브러리이다. 특히 숫자 Table과 시계열을 조작하기 위한 데이터 구조와 연산을 제공한다.
 - Pandas의 대표적인 Data object는 2가지가 있다.
 
  ### 1.1.1 Series 
  Series는 1차원 배열의 형태이고 index라는 한 가지 기준에 의하여 데이터가 저장된다.<br>
  Dictionary와 비슷하게 index와 value가 1:1 대응이다.<br>
  Series는 정수형 index 이름형 index 모두 접근 가능하다.<br>

![series](https://user-images.githubusercontent.com/81912557/137123437-69851aac-39ec-403a-88d5-7d6092a40270.PNG)
       
  ### 1.1.2 DataFrame
  Dataframe은 2차원 배열의 형태를 갖는다. index와 column이라는 두 가지 기준에 의하여 표 형태처럼 Data가 저장된다.<br>
  흔히 알고 있는 Table형태와 동일하다.<br>
![dataframe](https://user-images.githubusercontent.com/81912557/137123523-056f23e0-c8fc-44eb-b250-9e70a96ef0a7.PNG)<br>
- DataFrame은 다양한 format으로 import.export하여 다른 파일을 읽어올 수 있다.(csv,excel,json 등)
- DataFrame.loc[인덱스 이름] or DataFrame.iloc[정수형 위치 인덱스]로 행에 대해 접근할 수 있다.
- DataFrame[열이름] or DataFrame[정수형 위치 인덱스]로 열에 대해 접근할 수 있다.<br>

Pandas는 다양한 함수를 지원한다.<br>

- read_excel()<br>
read_excel()을 통해 excel 파일을 DataFrane 구조로 가져올 수 있다.
![pandas_read](https://user-images.githubusercontent.com/81912557/137126426-fee00fd3-5ac0-44a7-a1d1-bad6c9b8fad3.PNG)
- info()<br>
DataFrame의 정보를 확인할 수 있다.<br>
![info](https://user-images.githubusercontent.com/81912557/137126512-574864c4-63e2-4bf1-a69e-2a75e05f13bd.PNG)
- describe()<br>
DataFrame의 기술통계적인 부분을 확인할 수 있다.<br>
![des](https://user-images.githubusercontent.com/81912557/137126481-141b2df1-43e1-49e6-88e8-c0f24bcbde74.PNG)<br>

- 위의 horsepower 컬럼의 NaN 값이 있으므로 결측치거 있음을 알 수 있다. -> 해당 컬럼은 float형태인데 결측값이 ?로 들어가서 NaN이 나온 상황

      결측치 처리 방법
      1.평균 값으로 대체
      2.numpy.float으로 형변환
      3.numpy.nan으로 교체

  
           
 ## 1.2. Seaborn
 ## 1.3. Matplotlib




