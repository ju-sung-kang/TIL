## C언어의 컴파일과정

https://gracefulprograming.tistory.com/16

1. #include #define 등을 처리하는 전처리 과정을 전처리기가 수행
2. 컴파일러가 고레벨 코드를 어셈블리어 코드로 바꿔줌
3. 어셈블러가 어셈블리어 코드를 기계어(바이트코드)로 바꿔줌
4. 링커가 표준라이브러리(printf, scanf ...)와 사용자 라이브러리들을 링크함
