번역하면 독립성 

독립성은 응집도와 결합도로 측정한다. 

모듈의 독립성이 높을 수록?
1. 수정 시  다른 모듈에 끼치는 영향이 적음. 
2. 오류가 발생하더라도 쉽게 문제를 발견함.

결합도(Coupling)
응집도(Cohesion)

모듈의 독립성을 높이려면?
1. 결합도를 낮춘다.
2. 응집도를 높인다. 

결합도의 단계
1. 자료 결합도 (Data) 
	=> 패러미터 등으로 자료를 활용. 
2. 스탬프 결합도 (Stamp)
	=> 객체 등으로 참조 
3. 제어 결합도(Control) 
	=> 제어 요소에 영향을 줌 
4. 외부 결합도 (External)
	=> 모듈이 외부의 데이터를 참조
5. 공통 결합도 (Common)
	=> 전역변수등을 참조 
6. 내용 결합도 (Content)
	=> 내부 기능과 데이터를 직접참조 

그럼 결국은 

파라미터 < Object, Array < 제어 로직 < 외부 데이터 < 전역변수 < 내부 기능과 데이터
순으로 결합도를 낮출 때 사용하지 말아야 하는 순서 

결합도는 의존도와 같은 말이다. 

응집도의 단계 
1. 기능적 응집도
	=> 모듈 내의 모든 요소들이 하나의 기능을 수행하기 위해 구성
2. 순차적 응집도
	=> 한 요소의 출력이 다른 요소의 입력으로 사용됨 
3. 통신적 응집도
	=> 동일한 입력 과 출력데이터를 사용해 서로 다른 기능을 수행하는 경우 
4. 절차적 응집도
	=> 순차적으로 수행되지만, 흐름 제어요소가 전달됨 (데이터가 아니라) 
5. 일시적 응집도
	=> 순서에 상관없이 특정 시점에 반드시 수행됨 
6. 논리적 응집도
	=> 논리적으로 비슷한 기능을 수행하지만, 서로의 관계는 밀집하지 않은 형태
7. 우연적 응집도 
	=> 아무런 관련없이 구성된 형태 


각 단계 별 차이가 느껴져야 하는데 .. 응집도가 좀 어려운 것 같다. 

