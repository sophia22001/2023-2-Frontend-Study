<1장-자바스크립트 개요>
1-1-1.프로그래밍 언어: 컴퓨터 프로그램을 작성하기 위한 언어
컴파일: 소스코드를 실행하기 앞서 기계어로 번역하는 행위
인터프리터 언어: 프로그램을 한 줄마다 기계어로 번역하는 프로그래밍 언어
프로그래밍 언어의 유형: 절차적 언어, 객체 지향 언어,함수형 언어, 논리형 언어

1-1-2.자바스크립트 특징
자바스크립트는 인터프리터 언어이다.
동적 프로토타입 기반 객체 지향 언어이다.-객체 생성 후에도 프로퍼티와 메서드를 동적으로 추가/삭제 가능
동적 타입 언어이다.-변수 타입이 없다.
함수가 일급 객체이다.-자바 스크립트의 함수는 객체이다.함수형 프로그래밍 가능
함수가 클로저를 정의한다.

1-1-3.자바스크립트의 기술적 요소
1.코어 언어-ECMAScript
2.클라이언트 측의 고유한 기술 요소: window인터페이스, DOM, XMLHttpRequest
3.서버 측 자바스크립트의 고유한 기술 요소: Node.js, Rhino, Aptana Jaxer

1-1-4.ECMAScript 6

1-2.자바스크립트의 역사

<2장-프로그램의 작성법과 실행법>
2-2.간단한 예제
function fact(n){
  if(n<=1){
    return n;
  }
  return n*fact(n-1);
}
for(var i=1;i<10;i++){
  console.log(i+"!="+fact(i));
}


2-3.프로그램 실행법
//factorial.html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>팩토리얼 계산</title>
</head>
<body>
  <script>
    function fact(n){
      if(n<=1){
       return n;
    }
    return n*fact(n-1);
  }
  for(var i=1;i<10;i++){
    document.write(i+"! =" + fact(i) + "<br/>");
  }
  </script>
</body>
</html>

//factorial2.html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>팩토리얼 계산</title>
</head>
<body>
  <script src="./factorial.js"></script>
</body>
</html>

2-4.프로그램 작성법
2-4-1.문자 코드-유니코드 문자
2-4-2.대문자와 소문자 구별
2-4-3.토큰과 공백 문자
토큰: 프로그램을 구성하는 최소 단위->어휘분석, 구문분석
공백 문자: 토큰을 구분할 수 있게 함.
  프로그램 가독성 높이기
2-4-4.문장: 토큰을 나열하여 한 문장을 만들고, 문자을 이용해 컴퓨터에 명령을 내린다.
  ex> console.log( i + "! = " + fact(i));
복합문: 문장 여러 개를 중괄호{}로 감싼 코드
빈 문장: 문장이 하나도 없는 문장. 빈 문장을 세미콜론으로 작성한다.
세미콜론 자동 추가되는 경우가 있다.
2-4-5.주석: 프로그램의 소스 코드에 삽입하는 설명문 // or /* */

<3장.변수와 값>


