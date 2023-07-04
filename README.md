# spring5fs
스프링5 프로그래밍 입문 예제

1. 스프링 프레임워크의 주요 특징 4가지
  - 의존주입(Dependency Injection : DI) 지원
  - AOP(Aspect-Oriented Programming : 관점 지향 프로그래밍) 지원
  - MVC 웹 프레임워크 제공
  - JDBC, JPA 연동, 선언적 트랜잭션 처리 등 DB 연동 지원

2. 빌드 도구 2가지
  - Maven
  - Gradle

3. Maven
  - pom.xml : Maven 프로젝트에 대한 설정 정보(의존 모듈이나 플러그인 등)를 관리하는 파일

4. Maven 의존 설정
  - Maven은 한 개의 모듈을 아티팩트라는 단위로 관리
  - 의존 추가 : 일반적인 자바 어플리케이션에서 클래스 패스에 모듈을 추가한다는 것을 뜻함
  - 아티팩트명 : 아티팩트이름-버전.jar

5. Maven 리포지토리
  - Maven 로컬 리포지토리 폴더 : [사용자홈폴더]\.m2\repository
  - Maven 원격 중앙 리포지토리 : repo.maven.apache.org
  - 로컬 리포지토리에서 [그룹ID]\[아티팩트ID]\[버전] 폴더에 아티팩트이름-버전.jar 파일이 있는지 검사, 파일이 존재하면 이 파일을 사용
  - 로컬 리포지토리에 파일이 없으면 Maven 원격 중앙 리포지토리로부터 해당 파일을 다운로드하여 로컬 리포지토리에 복사한 뒤 그 파일을 사용
  - 파일 다운로드 테스트 : 명령 프롬트에서 프로젝트 폴더로 이동 후 'mvn compile' 명령 실행
    
6. Maven 의존 전이(Transitive Dependencies)
  - 의존 대상이 다시 의존하는 대상까지도 의존 대상에 포함(의존하는 대상뿐만 아니라 의존 대상이 다시 의존하는 대상도 함께 다운로드함)

7. Maven 기본 폴더 구조
  - src\main\java : 자바 소스 코드 폴더
  - src\main\resources : 자바 소스 이외의 자원 폴더(XML, 프로퍼티 파일 등)
  - src\main\webapp : 웹 어플리케이션 기준 폴더(JSP 소스 코드, WEB-INF\web.xml 파일 등)
