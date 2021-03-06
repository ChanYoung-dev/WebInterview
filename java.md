## 1.OOP란?
OOP전의 프로그래밍 패러다임을 살펴보면, 중심이 컴퓨터에 있었다. 컴퓨터가 사고하는대로 프로그래밍을 하는 것이다. 
하지만 객체지향 프로그래밍이란 인간 중심적 프로그래밍 패러다임이라고 할 수 있다. 
즉, 현실 세계를 프로그래밍으로 옮겨와 프로그래밍하는 것을 말한다. 현실 세계의 사물들을 객체라고 보고 그 객체로부터 개발하고자 하는 애플리케이션에 필요한 특징들을 뽑아와 프로그래밍 하는 것이다. 
이것을 추상화라고합니다. 이런 추상화와 같이 OOP으 핵심은 상속과 캡슐화, 다형성등이 있습니다.


### OOP의 핵심

Inheritance: 상속
- extends를 통해서 부모 클래스의 모든 속성과 메소드를 자식 클래스가 상속받는 것
- 코드중복을 줄이고 코드를 재사용 가능한 조각으로 나눌수 있다
- 이 덕분에 클래스를 더 작은 단위 Class로 쪼개고 분할하여 레고처럼 클래스들을 조립해서 부모클래스들의 코드들을 재사용할수 있다

Encapsulation: 캡슐화
- 데이터나 함수를 class안에 두는 것을 의미
- 어떻게 클래스 정보에 접근 혹은 수정하는지를 결정하는 권한을 제공
- 덕분에 데이터를 숨길수가 있고 노출할 자료와 숨길자료를 선택할 수 있다

Abstraction: 추상화
- 구현 세부 정보를 숨기는 일반 인터페이스를 지정하는 행위


Polymorphism: 다형성
- 같은 이름의 메소드가 클래스 혹은 객체에 따라 다르게 구현되는 것을 말합니다.
- 즉 슈퍼 클래스에 구현된 메소드를, 서브 클래스에서 자식의 특징에 맞게 동일한 이름으로 다시 구현하는 것인데 이것을 메소드 오버라이딩이라고 합니다

### OOP의 단점
객체 간의 정보 교환이 모두 메시지 교환을 통해 일어나므로 실행 시스템에 많은 overhead 가 발생하게 된다. 
하지만 이것은 하드웨어의 발전으로 많은 부분 보완되었다. 객체 지향 프로그래밍의 치명적인 단점은 함수형 프로그래밍 패러다임의 등장 배경을 통해서 알 수 있다. 
바로 객체가 상태를 갖는다는 것이다. 변수가 존재하고 이 변수를 통해 객체가 예측할 수 없는 상태를 갖게 되어 애플리케이션 내부에서 버그를 발생시킨다는 것이다. 
이러한 이유로 함수형 패러다임이 주목받고 있다.

## 2.객체 지향적 설계 원칙
- SRP(Single Responsibility Principle) : 단일 책임 원칙
  - 클래스는 단 하나의 책임을 가져야 하며 클래스를 변경하는 이유는 단 하나의 이유이어야 한다.
- OCP(Open-Closed Principle) : 개방-폐쇄 원칙
  - 확장에는 열려 있어야 하고 변경에는 닫혀 있어야 한다.
- LSP(Liskov Substitution Principle) : 리스코프 치환 원칙
  - 상위 타입의 객체를 하위 타입의 객체로 치환해도 상위 타입을 사용하는 프로그램은 정상적으로 동작해야 한다.
- ISP(Interface Segregation Principle) : 인터페이스 분리 원칙
  - 인터페이스는 그 인터페이스를 사용하는 클라이언트를 기준으로 분리해야 한다.
- DIP(Dependency Inversion Principle) : 의존 역전 원칙
  - 고수준 모듈은 저수준 모듈의 구현에 의존해서는 안된다.
