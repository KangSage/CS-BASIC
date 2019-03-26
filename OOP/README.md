# 객체 지향 프로그래밍 (Object Oriented Programming)

## SOLID (객체 지향 설계)

* 로버트 마틴이 2000년대 초반에 명명한 객체 지향 프로그래밍 및 설계의   
  다섯 가지 기본 원칙을 마이클 페더스가 두문자어 기억술로 소개한 것.
* 유지보수와 확장이 쉬운 시스템을 만들고자 할 때 이 원칙을 함께 적용할 수 있다.
* SOLID 원칙들은 소프트웨어 작업에서 프로그래머가 소스 코드가 읽기 쉽고 확장하기 쉽게 될 때까지  
  소스 코드를 리팩토링하여 코드 스멜`code smell`을 제거하기 위해 적용할 수 있는 지침이다.  
  이 원칙들은 애자일 소프트웨어 개발과 적응적 소프트웨어 개발의 전반적 전략의 일부다.

### 개요
* SRP - 단일 책임 원칙 (Single responsibility principle)  
  - 하나의 클래스는 하나의 책임만을 가져야한다.
* OCP - 개방 - 폐쇄 원칙 (Open / Closed Principle)  
  - 소프트웨어 요소는 확장에는 열려 있으나 변경에는 닫혀 있어야 한다.
* LSP - 리스코프 치환 원칙 (Liskov substitution principle)  
  - 프로그램 객체는 프로그램의 정확성을 깨뜨리지 않으면서 하위 타입의 인스턴스로 바꿀 수 있어야 한다. 
* ISP - 인터페이스 분리 원칙 (Interface segregation principle)
  - 특정 클라이언트를 위한 인터페이스 여러 개가 범용 인터페이스 하나보다 낫다.
* DIP - 의존관계 역전 원칙 (Dependency inversion principle)
  - 프로그래머는 "추상화에 의존해야지 구체화에 의존해선 안된다."  
    의존성 주입은 이 원칙을 따르는 방법 중 하나다.

### 5가지 원리의 핵심내용

#### A. SRP - 단일 책임 원칙 (Single responsibility principle)
> THERE SHOULD NEVER BE MORE THAN ONE REASON FOR A CLASS TO CHANGE.

1. 정의  
   작성된 클래스는 하나의 기능만 가지며 클래스가 제공하는 모든 서비스는  
   그 하나의 책임(변화의 축 : axis of change)을 수행하는데 집중 되어야 있어야 한다.  
   어떤 변화에 의해 클래스를 변경해야 하는 이유는 오직 하나뿐이어야 한다는 의미.  
   SRP 원리를 적용하면 무엇보다도 책임 영역이 확실해지므로 다른 책임으로 변경되는 연쇄작용에서 자유로울 수 있다.  
   책임을 적절히 분해하여 코드의 가독성 향상, 유지보수 용이라는 이점을 누릴 수 있고  
   객체지향 원리의 대전제 격인 OCP 원리와 다른 원리들을 적용하는 기초가 된다.  
   이 원리는 다른 원리들에 비해 개념은 비교적 단순하나 이 원리를 적용하여 직접 클래스를 설계하기란 쉽지 않다.  
   실무의 프로세스는 매우 복잡, 다양하고 변경 또한 빈번하므로 경험이 많지 않거나  
   도메인에 대한 업무 이해가 부족하면 SRP 원리와 멀어지게 된다.  
   따라서 평소에 항상 '책임'이라는 단어를 상기하는 연습과 경험이 필요한 원칙이다.
   
1. 적용 방법  
   리팩토링(Refactoring: Improving the Design of Existing Code - Martin Fowler)에서  
   소개하는 대부분의 위험 상황에 대한 해결법은 직간접적으로 SRP 원리와 관련있으며 이는 항상 코드를  
   최상으로 유지한다는 리팩토링의 근본 정신도 항상 객체들의 책임을 최상의 상태로 분배한다는 것에서 비롯된다.
   
   * 여러 원인에 의한 변경 (Divergent change):  
   Extract Class `추출한 클래스`를 통해 혼재된 각 책임을 각각의 개별 클래스로 분할하여  
   클래스당 하나의 책임만을 맡도록 하는 것. 여기서 관건은 


> 참고  
위키피디아 SOLID (객체 지향 설계)  
https://ko.wikipedia.org/wiki/SOLID_(%EA%B0%9D%EC%B2%B4_%EC%A7%80%ED%96%A5_%EC%84%A4%EA%B3%84)  
nextree 객체지향 개발 5대 원리: SOLID  
http://www.nextree.co.kr/p6960/

> 코드 스멜 : https://ko.wikipedia.org/wiki/%EC%BD%94%EB%93%9C_%EC%8A%A4%EB%A9%9C  
애자일 소프트웨어 개발 : https://ko.wikipedia.org/wiki/%EC%BD%94%EB%93%9C_%EC%8A%A4%EB%A9%9C  