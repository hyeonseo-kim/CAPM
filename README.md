# CAPM Analysis and Portfolio Risk Management

CAPM 분석과 포트폴리오 리스크 관리 실습 내용을 정리한 프로젝트입니다.  
과거 금융 데이터를 활용하여 자산 수익률, 시장 수익률, 베타, 초과수익률, VaR, 포트폴리오 최적화 등을 분석합니다.

## Project Overview

본 프로젝트는 개별 자산의 수익률이 시장 수익률과 어떤 관계를 가지는지 분석하고, CAPM(Capital Asset Pricing Model)을 통해 자산의 시장 민감도를 추정하는 것을 목표로 합니다.

또한 포트폴리오 관점에서 위험과 수익률을 함께 고려하여 투자 의사결정에 필요한 기초적인 리스크 분석을 수행합니다.

## Main Topics

- Historical stock return analysis
- Market return calculation
- CAPM regression
- Beta estimation
- Expected return and excess return
- Portfolio return and risk
- Value at Risk(VaR)
- Portfolio optimization
- Risk-return trade-off

## Methodology

본 프로젝트에서는 다음과 같은 분석 절차를 수행하였습니다.

1. 데이터 수집 및 전처리
   - 개별 주식 가격 데이터와 시장 지수 데이터 수집
   - 결측치 확인 및 정리
   - 가격 데이터를 수익률 데이터로 변환

2. 수익률 분석
   - 개별 자산의 일별 또는 월별 수익률 계산
   - 시장 수익률 계산
   - 평균 수익률과 변동성 확인

3. CAPM 회귀분석
   - 개별 자산의 초과수익률을 종속변수로 설정
   - 시장 초과수익률을 설명변수로 설정
   - 회귀분석을 통해 alpha와 beta 추정

4. 리스크 분석
   - 자산별 변동성 비교
   - VaR(Value at Risk)을 활용한 손실위험 측정
   - 포트폴리오 수익률과 위험 계산

5. 포트폴리오 최적화
   - 자산 간 공분산 구조 확인
   - 위험 대비 기대수익률을 고려한 포트폴리오 구성
   - 효율적 투자 조합 탐색

## CAPM Model

CAPM은 개별 자산의 기대수익률이 무위험수익률과 시장위험 프리미엄에 의해 설명된다고 보는 모형입니다.

```text
E(R_i) = R_f + β_i [E(R_m) - R_f]
