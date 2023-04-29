# 2장 의미 있는 이름

### 들어가면서
변수, 함수, 인수, 클래스, 패키지, 소스파일, 소스파일이 담긴 디렉터리, jar, war, ear파일 등 어디에나 쓰이는 이름을 잘 지어보자.<br/>
효과적으로 이름을 잘 짓는 법 16가지를 소개한다.

## 1.의도를 분명히 밝혀라
#### -변수(함수,클래스 등)의 존재 이유는?<br/> 
#### -수행 기능은?<br/>
#### -사용 방법은?<br/>
ex) int elapsedTimeInDays;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;int daysSinceCreation;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;int fileAgeInDays;<br/>

## 2.그릇된 정보를 피하라
#### -널리 쓰이는 약어 사용x                            
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) hp, aix, sco...<br/>
#### -특수한 의미를 가진 단어 사용x                      
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) List(대신 Accounts)<br/>
#### -흡사한 이름 사용x                                 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) XYZControllerForEfficientHandlingOfStrings / XYZControllerForEfficientStorageOfStrings <br/>
#### -일관성 떨어지는 표기법 사용x. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;유사한 개념은 유사한 표기법을 사용한다.<br/>
#### -비슷하게 생긴 이름 사용x                          
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) 소문자L : 숫자1, 대문자O : 숫자0 <br/>

## 3.의미 있게 구분하라
저자의 의도가 드러나게, 읽는 사람이 차이를 알도록 이름 짓기.

## 4.발음하기 쉬운 이름을 사용하라
발음하기 어려운 이름은 토론하기 어렵다. ex)class DtaRcrd102{...};

## 5.검색하기 쉬운 이름을 사용하라
긴 이름이 좋다. 이름 길이는 범위 크기에 비례해야한다.<br/>
달랑 문자 하나, 상수 사용x. <br/>
ex) const int WORK_DAYS_PER_WEEK = 5; 만약 달랑 5만 사용했으면 5가 들어가는 이름 모두 검색해야함.

## 6.인코딩을 피하라
인코딩한 이름은 발음하기 어렵고 오타가 생기기 쉬움.
#### 헝가리식 표기법 
변수 및 함수의 인자 이름 앞에 데이터 타입을 명시하는 코딩 규칙. ex) PhoneNumber phoneString;<br/>
IDE발전으로 컴파일 하지 않고도 타입오류를 감지할 수 있어 사용할 필요가 없어짐.<br/>
#### 멤버 변수 접두어
멤버 변수에 m_ 접두어를 붙일 필요 없음. 멤버 변수를 다른색상으로 표시해주는 IDE를 사용하면 그만.
#### 인터페이스 클래스와 구현 클래스(interface class, concrete class) 
인터페이스 이름에 접두어를 붙이지 않는 편이 좋다.<br/>
둘 중 하나를 인코딩 해야한다면 구현클래스를 택함.<br/>
ex) IShapeFactory > ShapeFactoryImp or CSHapeFactory 

## 7.자신의 기억력을 자랑하지 마라

## 8.클래스 이름

## 9.메서드 이름

## 10.기발한 이름은 피하라

## 11.한 개념에 한 단어를 사용하라

## 12.말장난을 하지마라 

## 13.해법 영역에서 가져온 이름을 사용하라

## 14.문제 영역에서 가져온 이름을 사용하라

## 15.의미 있는 맥락을 추가하라 

## 16.불필요한 맥락을 없애라

### 마치면서
