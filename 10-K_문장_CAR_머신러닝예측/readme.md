<io>
사업보고서 전체에 대해서 보는 것이 필요하나, 이미 이전의 단어 추출 기반으로 산업을 분류한 것과 유사하게, <br>
business description에서 나온 문장 단위에서 token화를 해 준 다음 unigrams와 bigrams를 기반으로 filling date 이후 CAR 을 예측해보고자 한다. <br>
대조군으로 Loughran and McDonald 사전 기반으로 긍정, 부정, 긍정부정 비율 등과 비교하여 결과의 정확도를 보고자 한다. <br>
머신러닝으로 사용한 모델은 SVR, RF, Gradient Boost, Decision Tree 등 이다. <br>

분석 결과, Random Forrest가 가장 적합한 것으로 나타났으며 <br>
각 행별로 열 값(unigrams, bigrams 전체 집합) 의 수가 47만개에 달한 탓에 <br>
배치 크기를 줄여야 될 뿐더러, GPU로 적합 역시 455개로 구성된 배치가 아니면 돌릴 수 없어 CPU 대비 성능의 효과를 보지 못하였다. <br>
텍스트요약 딥러닝 기법등을 활용하여 열 수를 줄인다면 GPU에서의 이점 등도 관찰 가능할 것으로 기대된다. <br>
또한, 전체 10-K에 대해서 기업의 매출 내역 등에 서술하는 부분에 있어서도 긍정/단어 혹은 기타 단어들을 추가한다면 정확도도 더 높아질 것이다.
