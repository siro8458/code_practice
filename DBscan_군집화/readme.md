DBscan과 K-means clustering을 기반으로 조금 더 정확한 군집화를 해보고자 함 <br>
제약조건(각 지역별 최대 면적) 등을 기반으로 Constrained K-Means Clustering 논문과 유사하게 해보고자 노력함 <br>
주로 밀도 군집화 등에 사용되는 geomtry 데이터를 기반으로 하고자 함 <br>

따라서 브이월드 중에서 교육환경구역에 대한 데이터를 멀티프로세스를 통하여 받아오고
DBscan을 통하여 군집화 후 기준에 따른 제약적인 clustering을 통하여 효율적인 면적 및 군집 구분에 대해서 분석을 진행함
