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
#### -헝가리식 표기법 
변수 및 함수의 인자 이름 앞에 데이터 타입을 명시하는 코딩 규칙. ex) PhoneNumber phoneString;<br/>
IDE발전으로 컴파일 하지 않고도 타입오류를 감지할 수 있어 사용할 필요가 없어짐.<br/>
#### -멤버 변수 접두어
멤버 변수에 m_ 접두어를 붙일 필요 없음. 멤버 변수를 다른색상으로 표시해주는 IDE를 사용하면 그만.
#### -인터페이스 클래스와 구현 클래스(interface class, concrete class) 
인터페이스 이름에 접두어를 붙이지 않는 편이 좋다.<br/>
둘 중 하나를 인코딩 해야한다면 구현클래스를 택함.<br/>
ex) IShapeFactory > ShapeFactoryImp or CSHapeFactory 

## 7.자신의 기억력을 자랑하지 마라
문자 하나만 사용하는 변수 이름 x(루프 범위가 작고 다른 이름과 충돌하지 않을때만 가능.)<br/>
명료하게 남들이 이해하는 코드를 써라.

## 8.클래스 이름
#### -클래스나 객체이름은 명사나 명사구로 써라. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) Customer, WikiPage, Account, AddressParser 등
#### -Manager,Processor,Data,Info 등과 같은 단어 피하기.
#### -동사 사용x 

## 9.메서드 이름
#### 동사나 동사구가 적합하다.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex) postPayment, deletePage, save 등
#### 접근자, 변경자, 조건자는 javadean 표준에 따라 값 앞에 get, set, is를 붙인다.
String name = employee.getName();<br/>
customer.setName("mike");<br/>
if(paycheck.isPosted())...<br/>

## 10.기발한 이름은 피하라
특정 문화에서만 사용하는 농담 피하기.<br/>
구어체나 속어 x.

## 11.한 개념에 한 단어를 사용하라
메서드 이름은 독자적이고 일관적이어야한다. (주석을 뒤져보지 않게 해야함...)<br/>
같은 메서드를 클래스마다 fetch, retrieve, get 등 제각각 부르면 안됨.<br/>

## 12.말장난을 하지마라 
한 단어를 두 가지 목적으로 사용x.<br/> 
ex) add() : 기존값 두개를 더하거나 이어서 새로운 값을 만드는 메서드.<br/>
집합에 값 하나를 추가하는 메서드를 만들때, 일관성을 지킨답시고 add 사용 금지. insert나 append가 적당.

## 13.해법 영역에서 가져온 이름을 사용하라
프로그래머에게 익숙한 용어를 사용해도 괜찮다. <br/>
전산용어, 알고리즘 이름, 패턴이름, 수학용어 등등..<br/>
해법영역: 프로그래머 전문 용어인듯?

## 14.문제 영역에서 가져온 이름을 사용하라
적절한 프로그래머 용어가 없다면 문제 영역에서 이름을 가져온다.<br/>
문제 영역: 분야 전문 용어인듯?

## 15.의미 있는 맥락을 추가하라 
클래스, 함수, 이름공간에 맥락을 부여한다. 안된다면 접두어를 붙인다.<br/>
firstName ,lastName, steet, city, state... 등 주소를 보여주는 변수가 있다. <br/>
addr라는 접두어를 추가해 addrFirstName ,addrLastName, addrSteet, addrCity, addrState로 나타내주면 맥락이 분명해짐.<br/>
물론 Address 클래스를 생성하면 더 좋음.<br/>

## 16.불필요한 맥락을 없애라
의미가 분명한 경우에 한해서 짧은 이름보다 긴이름이 좋다. <br/>
ex) Gas Station Deluxe라는 애플리케이션을 만들때 모든 클래스 이름을 GSD로 시작하면.....쫌..

### 마치면서
소개한 규칙을 적용해서 가독성을 높여보자.<br/>
다른 사람이 짠 코드를 손본다면 리팩터링 도구를 사용해 문제 해결 목적으로 이름을 개선하자.<br/>
