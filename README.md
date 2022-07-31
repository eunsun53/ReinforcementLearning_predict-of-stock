# ReinforcementLearning_predict-of-stock

* model- free RL, Q-Learning 적용
  : agent가 (state, action) 에 따른 reward로 피드백을 받아 최대의 보상을 받을 수 있도록 Q 함수를 업데이트 할 수 있도록 policy를 찾아내도록 하는 것
  
#Building Environment


* state: [(해당 주식 갯수, 해당 주식 1주당 가격), 계좌 잔액]
> action: sell(0), hold(1), buy(2)
> reward: 보상을 주는 policy는 다양하게 상황에 맞게 정의함

>> action이후의 포트폴리오의 가치가 높으면 +1, 낮으면 -1 feedback
>> action이후의 포트폴리오의 가치가 높으면 +1, 낮으면 -100 feedback
>> action이후의 포트폴리오의 가치의 차이만큼 feedback  
