# Programmers_42839
## 프로그래머스 - 소수찾기 (https://programmers.co.kr/learn/courses/30/lessons/42839)
재귀를 이용한 완전탐색으로 풀 수 있었던 문제.
문제를 보자마자 재귀를 이용해야 함은 알았으나,, 
중복 문자를 제거해가며 모든 조합을 어떻게 효율적으로 만들 수 있을지 생각해보다가 substring을 사용.
소수 검증 로직은 몇몇가지 조건으로 예외 처리 후, 제곱근 값까지만 확인.
앞에 0이 붙은 문자열의 경우 int로 parsing 시, 기존에 확인한 정수와 동일한 수 있어, 
중복된 값은 무시할 수 있게 D.T. 는 HashSet으로 사용

구현 순서는 아래와 같다 : 
1. Input 문자열을 쪼개 모든 조합을 만들 수 있는 재귀함수 구현
2. 소수인지 검증하는 메소드 구현
3. 소수일 경우는 HashSet에 추가, 결과값으로 HashSet 크기 반환

