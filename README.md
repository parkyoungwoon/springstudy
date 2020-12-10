# springstudy
스프링 공부

# study

참고 사이트
-- pom.xml 양식 다운받는 사이트
https://mvnrepository.com/

공부한 내용

spring 관련

spring 특징
- POJO 기반의 구성 
- 의존성 주입(DI)을 통한 객체 간의 관계 구성
- AOP 지원(Aspect-Oriented_Programming)
- MVC 구조
- WAS에 종속적이지않은 개발 환경
*POJO 특수한 기술에 종속되지 않은 환경
*AOP 관점지향프로그래밍 : 쉽게 말하면 객체지향프로그래밍을 하더라도 프로그램이 커지면 중복되는 경우가 생길수밖에없음
*                       중복되는 코드를 줄이기 위하여 xml 이나 설정 자체를 해당 로직을 타게 하는 것이라고 생각하면 될듯(AspectJ, Spring AOP 를 공부하면 좋음)
* 의존성 주입(DI) : inner function 생각하면 쉬움, A객체가 없으면 B객체의 실행이 불가능한 것을 의미함

어노테이션
-> 컴파일러가 특정 오류를 억제하도록 지시하는 것과 같이 프로그램 코드의 일부가 아닌 
프로그램에 관한 데이터를 제공, 코드에 정보를 추가하는 정형화된 방법.
@붙여서 클래스 위에 쓰느거 생각하면 됨

root-context.xml : 스프링 프레임워크를 관리해야 하는 객체

spring 실행 순서(이정도만 일단 알고있으면 될듯)
1. 웹 어플리케이션이 실행되면 web.xml 로딩
2. web에 등록되어 있는 ContextLoaderListener(Java Class) 생성
3. 생성된 ContextLoaderListener는 root-context.xml을 Loading
4. root-context.xml에 등록되어 있는 Spring Container가 구동

DB 라이브러리 설정
root-context 에서 설정
스프링이로딩되면서 읽어 들이는 문서이므로 주로 만들어진 클래스들은 이용해서 스프링의 빈으로 등록할 때 사용됨

자바에서 설정할 경우
@Bean 어노테이션을 이용하여 등록함

MyBatis 연동

실행되는 과정
String <-> MyBatis <-> DB

MyBatis 의 핵심 객체
SQLSessionFactory는 SQLSession를 생성해내는 객체
SQLSession를 이용하여 Connection을 생성하거나 SQL을 전달 리턴받는 구조로 작성



현재 스프링 97페이지까지 했음


