# 러스트 프로그래밍 언어

[들어가기 앞서](foreword.md)
[소개](ch00-00-introduction.md)

## 시작하기

- [시작하기](ch01-00-getting-started.md)
    - [설치하기](ch01-01-installation.md)
    - [Hello, World!](ch01-02-hello-world.md)
    - [Hello, Cargo!](ch01-03-hello-cargo.md)

- [추리 게임 튜토리얼](ch02-00-guessing-game-tutorial.md)

- [보편적인 프로그래밍 개념](ch03-00-common-programming-concepts.md)
    - [변수와 가변성](ch03-01-variables-and-mutability.md)
    - [데이터 타입들](ch03-02-data-types.md)
    - [함수 동작 원리](ch03-03-how-functions-work.md)
    - [주석](ch03-04-comments.md)
    - [제어문](ch03-05-control-flow.md)

- [소유권 이해하기](ch04-00-understanding-ownership.md)
    - [소유권이 뭔가요?](ch04-01-what-is-ownership.md)
    - [참조자와 빌림](ch04-02-references-and-borrowing.md)
    - [슬라이스](ch04-03-slices.md)

- [연관된 데이터들을 구조체로 다루기](ch05-00-structs.md)
    - [구조체를 정의하고 생성하기](ch05-01-defining-structs.md)
    - [구조체를 이용한 예제 프로그램](ch05-02-example-structs.md)
    - [메소드 문법](ch05-03-method-syntax.md)

- [열거형과 패턴 매칭](ch06-00-enums.md)
    - [열거형 정의하기](ch06-01-defining-an-enum.md)
    - [`match` 흐름 제어 연산자](ch06-02-match.md)
    - [`if let`을 사용한 간결한 흐름 제어](ch06-03-if-let.md)

## 기초적인 러스트 사용하기

- [모듈](ch07-00-modules.md)
    - [`mod`와 파일 시스템](ch07-01-mod-and-the-filesystem.md)
    - [`pub`으로 가시성 제어하기](ch07-02-controlling-visibility-with-pub.md)
    - [`use`로 이름 가져오기](ch07-03-importing-names-with-use.md)

- [일반적인 컬렉션](ch08-00-common-collections.md)
    - [벡터](ch08-01-vectors.md)
    - [스트링](ch08-02-strings.md)
    - [해쉬맵](ch08-03-hash-maps.md)

- [에러 처리](ch09-00-error-handling.md)
    - [`panic!`과 함께하는 복구 불가능한 에러](ch09-01-unrecoverable-errors-with-panic.md)
    - [`Result`와 함께하는 복구 가능한 에러](ch09-02-recoverable-errors-with-result.md)
    - [`panic!`이냐, `panic!`이 아니냐, 그것이 문제로다](ch09-03-to-panic-or-not-to-panic.md)

- [제네릭 타입, 트레잇, 그리고 라이프타임](ch10-00-generics.md)
    - [제네릭 데이터 타입](ch10-01-syntax.md)
    - [트레잇: 공유 동작을 정의하기](ch10-02-traits.md)
    - [라이프타임을 이용한 참조자 유효화](ch10-03-lifetime-syntax.md)

- [테스팅](ch11-00-testing.md)
    - [테스트 작성하기](ch11-01-writing-tests.md)
    - [테스트 실행하기](ch11-02-running-tests.md)
    - [테스트 조직화](ch11-03-test-organization.md)

- [I/O 프로젝트: 커맨드 라인 프로그램 만들기](ch12-00-an-io-project.md)
    - [커맨드 라인 인자 허용하기](ch12-01-accepting-command-line-arguments.md)
    - [파일 읽기](ch12-02-reading-a-file.md)
    - [모듈성과 에러처리의 향상을 위한 리팩토링](ch12-03-improving-error-handling-and-modularity.md)
    - [테스트 주도 개발로 라이브러리의 기능 개발하기](ch12-04-testing-the-librarys-functionality.md)
    - [환경 변수들을 활용하기](ch12-05-working-with-environment-variables.md)
    - [표준출력 대신 표준에러로 에러메시지 출력하기](ch12-06-writing-to-stderr-instead-of-stdout.md)

## 러스트로 생각하기

- [함수형 언어의 특성들: 반복자들과 클로저들](ch13-00-functional-features.md)
    - [클로저: 환경을 캡쳐할 수 있는 익명 함수](ch13-01-closures.md)
    - [반복자로 일련의 항목들 처리하기](ch13-02-iterators.md)
    - [I/O 프로젝트 개선하기](ch13-03-improving-our-io-project.md)
    - [성능 비교하기: 루프 vs. 반복자](ch13-04-performance.md)

- [More about Cargo and Crates.io](ch14-00-more-about-cargo.md)
    - [Customizing Builds with Release Profiles](ch14-01-release-profiles.md)
    - [Publishing a Crate to Crates.io](ch14-02-publishing-to-crates-io.md)
    - [Cargo Workspaces](ch14-03-cargo-workspaces.md)
    - [Installing Binaries from Crates.io with `cargo install`](ch14-04-installing-binaries.md)
    - [Extending Cargo with Custom Commands](ch14-05-extending-cargo.md)

- [스마트 포인터](ch15-00-smart-pointers.md)
    - [`Box<T>`는 힙에 있는 데이터를 가리키고 알려진 크기를 갖습니다](ch15-01-box.md)
    - [`Deref` 트레잇은 참조자를 통하여 데이터로의 접근을 허용합니다](ch15-02-deref.md)
    - [`Drop` 트레잇은 메모리 정리 코드를 실행시킵니다](ch15-03-drop.md)
    - [`Rc<T>`, 참조 카운팅 스마트 포인터](ch15-04-rc.md)
    - [`RefCell<T>`와 내부 가변성 패턴](ch15-05-interior-mutability.md)
    - [순환 참조를 만드는 것과 메모리 누수는 안전한 것에 해당됩니다](ch15-06-reference-cycles.md)

- [겁없는 동시성](ch16-00-concurrency.md)
    - [스레드](ch16-01-threads.md)
    - [메세지 패싱](ch16-02-message-passing.md)
    - [공유 상태](ch16-03-shared-state.md)
    - [확장 가능한 동시성: `Sync`와 `Send`](ch16-04-extensible-concurrency-sync-and-send.md)

- [Object Oriented Programming Features of Rust](ch17-00-oop.md)
    - [Characteristics of Object-Oriented Languages](ch17-01-what-is-oo.md)
    - [Using Trait Objects that Allow for Values of Different Types](ch17-02-trait-objects.md)
    - [Implementing an Object-Oriented Design Pattern](ch17-03-oo-design-patterns.md)

## 고급 주제

- [값의 구조와 매칭되는 패턴](ch18-00-patterns.md)
    - [패턴이 사용될 수 있는 모든 곳](ch18-01-all-the-places-for-patterns.md)
    - [반증 가능성: 패턴의 매칭이 실패할 수도 있는 경우](ch18-02-refutability.md)
    - [All the Pattern Syntax](ch18-03-pattern-syntax.md)

- [Advanced Features](ch19-00-advanced-features.md)
    - [Unsafe Rust](ch19-01-unsafe-rust.md)
    - [Advanced Lifetimes](ch19-02-advanced-lifetimes.md)
    - [Advanced Traits](ch19-03-advanced-traits.md)
    - [Advanced Types](ch19-04-advanced-types.md)
    - [Advanced Functions & Closures](ch19-05-advanced-functions-and-closures.md)

- [마지막 프로젝트: 멀티스레드 웹서버 만들기](ch20-00-final-project-a-web-server.md)
    - [싱글 스레드 웹서버](ch20-01-single-threaded.md)
    - [싱글 스레드 서버를 멀티스레드 서버로 바꾸기](ch20-02-multithreaded.md)
    - [우아한 종료와 정리](ch20-03-graceful-shutdown-and-cleanup.md)

- [Appendix](appendix-00.md)
    - [A - Keywords](appendix-01-keywords.md)
    - [B - Operators and Symbols](appendix-02-operators.md)
    - [C - Derivable Traits](appendix-03-derivable-traits.md)
    - [D - Macros](appendix-04-macros.md)
    - [E - Translations](appendix-05-translation.md)
    - [F - Newest Features](appendix-06-newest-features.md)
    - [G - How Rust is Made and “Nightly Rust”](appendix-07-nightly-rust.md)
