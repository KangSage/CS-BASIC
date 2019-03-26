# 객체 지향 프로그래밍 (Object Oriented Programming)

## SOLID (객체 지향 설계)

* 로버트 마틴이 2000년대 초반에 명명한 객체 지향 프로그래밍 및 설계의   
  다섯 가지 기본 원칙을 마이클 페더스가 두문자어 기억술로 소개한 것.
* 유지보수와 확장이 쉬운 시스템을 만들고자 할 때 이 원칙을 함께 적용할 수 있다.
* SOLID 원칙들은 소프트웨어 작업에서 프로그래머가 소스 코드가 읽기 쉽고 확장하기 쉽게 될 때까지  
  소스 코드를 리팩터링하여 코드 스멜```code smell```을 제거하기 위해 적용할 수 있는 지침이다.  
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

> 참고 문헌  
위키피디아 SOLID (객체 지향 설계)  
https://ko.wikipedia.org/wiki/SOLID_(%EA%B0%9D%EC%B2%B4_%EC%A7%80%ED%96%A5_%EC%84%A4%EA%B3%84)

> 코드 스멜 : https://ko.wikipedia.org/wiki/%EC%BD%94%EB%93%9C_%EC%8A%A4%EB%A9%9C  
애자일 소프트웨어 개발 : https://ko.wikipedia.org/wiki/%EC%BD%94%EB%93%9C_%EC%8A%A4%EB%A9%9C  
