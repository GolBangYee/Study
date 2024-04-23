# 인스턴스 생성 방식
```java
String str1 = new String("simple");
String str2 = "The Best String";
```
두 구문 모두 자바에서 String 인스턴스를 생성하는 방법이다.

# 참조값
```java
String str1 = "The Best String";
String str2 = "The Best String";

if(str1==str2)
  // ??
```
+ 놀랍게도 str1, str2는 `==`에서 true값으로 평가된다. 어짜피 같은 문자열이므로 str1을 str2가 가르키는 식으로 처리되기 때문
+ 참고로 참조 변수끼리에서 `==`연산은 참조값(주소값)으로 비교 연산이 진행된다.

```java
String str1 = new String("simple");
String str2 = new String("simple");

if(str1==str2)
//??
```
+ 위 코드의 str1과 str2는 서로 다르다고 평가된다.

# Immutable
+ Java에서 String의 문자열 값은 변경 불가능하다.
