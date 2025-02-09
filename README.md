# 자동차 경주

## 기능 목록
- [X] 경주할 자동차 이름 문자열과 경주 시도 횟수 입력 받기
- [X] 경주할 자동차 이름 문자열 파싱
  > 쉼표(,)를 기준으로 자동차 이름을 구분한다.
- [X] 잘못된 입력에 대한 예외 처리
  + 경주할 자동차 이름 입력 예외 처리
    > 특정 자동차 이름이 공백이거나 6글자 이상일 경우, IllegalArgumentException을 발생시킨다.
  + 경주 시도 횟수 입력 예외 처리
    > 경주 시도 횟수가 자연수가 아닐 경우, IllegalArgumentException을 발생시킨다.
- [X] 경주 진행 기능
  + 이동 여부 결정
    > 0에서 9 사이에서 구한 무작위 값이 4 이상일 경우, 이동한다.
  + 차수별 경주 시도 결과 저장
    > 경주를 시도할 때마다 경주 결과를 StringBuilder에 추가한다.
- [X] 경주 결과 출력
  + 최종 우승자 선정
    > 가장 많이 전진한 자동차를 우승자로 선정한다. (공동 우승 가능)
  + 차수별 경주 시도 결과와 우승자 안내 문구 출력