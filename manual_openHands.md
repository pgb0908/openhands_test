# openhands_test 프로젝트 메뉴얼

## 1. 프로젝트 개요

`openhands_test` 프로젝트는 Gradle을 사용하여 빌드되는 Java 기반의 웹 애플리케이션입니다. Spring Boot 프레임워크를 활용하여 RESTful API를 제공하는 예제 코드를 포함하고 있습니다.

## 2. 프로젝트 구조

```
openhands_test/
├── build.gradle
├── gradle/
│   └── wrapper/
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradlew
├── gradlew.bat
├── readme.md
├── settings.gradle
└── src/
    ├── main/
    │   ├── java/
    │   │   └── com/
    │   │       └── example/
    │   │           └── demo/
    │   │               ├── DemoApplication.java
    │   │               └── HelloController.java
    │   └── resources/
    │       └── application.properties
    └── test/
        └── java/
            └── com/
                └── example/
                    └── demo/
                        └── DemoApplicationTests.java
```

## 3. 주요 파일 설명

*   **`src/main/java/com/example/demo/DemoApplication.java`**: Spring Boot 애플리케이션의 메인 클래스입니다. 애플리케이션 실행의 시작점 역할을 합니다.
*   **`src/main/java/com/example/demo/HelloController.java`**: 기본적인 웹 요청을 처리하는 컨트롤러입니다. `/hello` 경로로 접속 시 "Hello!" 메시지를 반환합니다.
*   **`src/main/resources/application.properties`**: 애플리케이션의 설정 파일입니다. 서버 포트 등 다양한 설정을 정의할 수 있습니다.
*   **`build.gradle`**: Gradle 빌드 스크립트 파일입니다. 프로젝트의 의존성 관리 및 빌드 설정을 담당합니다.

## 4. 애플리케이션 실행 방법

1.  **Gradle Wrapper를 이용한 빌드 및 실행**:
    터미널에서 프로젝트 루트 디렉토리(`openhands_test`)로 이동한 후 다음 명령어를 실행합니다.

    ```bash
    ./gradlew bootRun
    ```

    이 명령어는 프로젝트를 빌드하고 내장된 Tomcat 서버를 사용하여 애플리케이션을 실행합니다.

2.  **직접 실행 (IDE 사용 시)**:
    `DemoApplication.java` 파일을 IDE에서 열고 `main` 메소드를 실행합니다.

## 5. API 엔드포인트

*   **`GET /hello`**: "Hello!" 메시지를 반환합니다.

## 6. 설정

`src/main/resources/application.properties` 파일에서 다음과 같은 설정을 변경할 수 있습니다.

*   **서버 포트**: `server.port=53001` (기본값은 53001입니다. 필요에 따라 변경하세요.)

## 7. 추가 정보

*   이 메뉴얼은 프로젝트의 기본적인 구조와 실행 방법을 안내합니다.
*   더 자세한 내용은 각 파일의 주석이나 Spring Boot 공식 문서를 참고하시기 바랍니다.