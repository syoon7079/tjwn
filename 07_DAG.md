6팀 서주 서윤,주원: 같이 화살표 목록을 작성하였으나, 업로드는 서윤이가 담당하였습니다.
서윤: B-1, B-3의 일부분 작성 주원: B-2업로드, B-3의 일부분 작성

노출변수: 저학력 정의: edu <=2 

B-1. 화살표 목록
age → edu*          (출생 코호트: 고령층일수록 학력이 낮음)
age → htn
sex → edu*          (고령 코호트에서 성별 학력 격차)
sex → htn
edu → income
edu → smk, drink, exercise
edu → bmi
income → bmi
smk, drink, exercise, bmi → htn
income → htn
htn → income*       (역방향: 질병으로 인한 근로 제한)

B-1. 네 유형으로 분류
| 변수 | 유형 | 근거 (한 줄) |
| age | 교란 | 연령이 학력 분포(코호트)와 혈압 양쪽의 원인이다 |
| sex | 교란 | 성별이 학력 격차와 고혈압 위험 양쪽에 영향을 준다 |
| income | 매개 | 학력이 소득을 결정하고 소득이 건강 자원을 통해 혈압에 닿는다 |
| bmi | 매개 | 학력 → 식습관 → 체중 → 혈압으로 가는 통로다 |
| smk / drink / exercise | 매개 | 학력 이후에 형성되는 행동이고 혈압으로 가는 통로다 |

B-1.보정집합 결정
1)보정해야 할 변수 (교란변수): {age, sex}
원인: age와 sex는 노출(edu)과 결과(htn) 모두에 공통 원인으로 작용하여 교란 경로(Backdoor Path: edu ← age → htn, edu ← sex → htn)를 형성하므로 반드시 보정해야한다.

2) 보정에서 제외해야 할 변수 (매개변수): {income, bmi, smk, drink, exercise}
원인: 이 변수들은 노출(edu)이 결과(htn)에 영향을 미치는 인과 경로 상에 위치한 매개변수(Mediator)이다. 매개변수를 보정할 경우 교육의 전체 인과 효과(Total Effect)가 왜곡( 과소평가/과잉보정 편향)되므로 보정집합에서 제외한다.

B-2. 
















