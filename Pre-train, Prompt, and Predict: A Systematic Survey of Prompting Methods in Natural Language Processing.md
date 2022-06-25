# Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing

### 먼저 Prompt-based learning 이란?
* 기존의 특정 태스크에 대한 supervised learning의 경우 input $x$를 받아서 output $y$를 predict하는 식으로 학습한다. 그러나 Prompt-based learning의 경우 텍스트 자체에 대한 예측을 그대로 사용하는 방식으로 모델링한다. 따라서 prediction 할 때 original input $x$를 template을 이용해 빈 칸이 있는 텍스트 $x'$으로 modify한 후 언어모델이 이 빈 칸을 채우도록 해서 결과값 $x^$를 얻고 여기서 최종 $y$값을 도출해 낸다.
* 이 방식의 장점
  - 대량의 raw text로 학습이 가능
  - 새로운 prompting function을 정의하면 모델이 few-shot 혹은 zero-shot으로 태스크 수행 가능
