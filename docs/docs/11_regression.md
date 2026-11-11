C-1 DAG: 정의표의 노출, 결과, 공변량을 모두 넣은 DAG 그리기(dagitty.net 캡처).
<img width="1875" height="1128" alt="11주차 DAG 그림" src="https://github.com/user-attachments/assets/ef118578-2e3b-4b87-baa0-331437a17b44" />
dagitty.net에 넣은 코드
dag {
  EatOut [exposure]  BMI [outcome]  U [latent]
  Age -> {Educ Income Work HH1 EatOut BMI PA Smoking Alcohol}
  Sex -> {Income Work EatOut BMI PA Smoking Alcohol}
  Educ -> {Income Work EatOut BMI PA Smoking Alcohol}
  Region -> {Income Work EatOut BMI}
  Work -> {Income EatOut BMI Alcohol}
  Income -> {EatOut BMI}
  HH1 -> {EatOut BMI}
  U -> {EatOut PA Smoking}
  PA -> BMI
  Smoking -> BMI
  EatOut -> {Alcohol Energy BMI}
  Alcohol -> BMI
  Energy -> BMI
}
C-1: 화살표마다 근거(시간 순서, 선행연구)를 말할 수 있어야 합니다.




C-1 역할 표와 보정집합: 공변량마다 교란·매개·충돌부 가운데 어느 역할인지와 근거를 적고, 추정 대상(총효과 또는 직접효과)에 맞는 최소 보정집합 정하기

완전 사례 표시: 보정변수가 모두 있는 사람을 표시하고 인원을 출력해, Table 1 분석 대상과 몇 명 차이 나는지 확인하기

C-2 회귀: 모형 1(노출만)과 모형 2(보정집합)를 같은 사람으로, 가중치·층·집락을 반영해 적합하기. 분석 대상 밖의 사람은 행을 지우지 않고 도메인으로 다루기

C-2 Table 2: 모형마다 계수 또는 오즈비, 95% 신뢰구간, p값, 분석 인원. 각주에 설계, 모형 종류, 보정변수, 결측 처리, 자료 이름과 연도 적기

C-3 해석: 관련성의 방향과 크기를 단위와 함께 쓰고, 보정 전후 변화를 DAG와 연결하기. 한계와 12주차에 해 볼 민감도분석 한두 가지 적기

역할 분담:

AI 사용 내역 정리:


























