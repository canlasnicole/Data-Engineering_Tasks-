# Data-Engineering_Tasks-

💳 Overseas Remittance Fraud Detection EDA
"Beyond the Box: Detecting the Anomaly Fingerprint in Global Transfers"

1. Project Overview (프로젝트 개요)
This project performs an Exploratory Data Analysis (EDA) on the Credit Card Fraud Detection dataset (OpenML ID: 42175). The goal is to identify patterns that distinguish fraudulent activity from normal user behavior to secure overseas remittance services.

본 프로젝트는 해외 송금 서비스의 보안 강화를 위해 사기 거래 패턴을 분석한 EDA 보고서입니다. OpenML의 데이터를 활용하여 정상 거래와 사기 거래의 통계적 차이를 규명합니다.

2. Key Findings & "Out-of-the-Box" Insights (주요 인사이트)
🕵️‍♂️ The "Quiet Hour" Vulnerability (시간적 공백)
While normal transactions peak during daylight hours, fraud density remains high during late-night "valleys." Criminals exploit periods of reduced human monitoring.
정상 거래가 적은 심야 시간대에 사기 거래 밀도가 유지되는 패턴을 발견했습니다. 이는 관리 공백기를 노린 공격임을 시사합니다.

💰 The "Low & Slow" Amount Trap (금액의 함정)
Fraudsters avoid high-value transfers that trigger automatic AML (Anti-Money Laundering) alarms. Instead, they focus on Middle-Value ($100-$500) transfers to stay under the radar.
고액 송금 대신 자동 탐지 시스템을 피하기 위한 $100~$500 사이의 '중간 금액' 사기 집중 현상을 확인했습니다.

3. Analysis Dashboard (분석 대시보드)
Our analysis includes advanced visualizations:

Missing Value Heatmap: Verified 100% data integrity.

Log-Scaled Distribution: Identified outliers in financial flows.

Comparative Density Plots: Visualized the separation between Normal and Fraud behaviors.

4. Business Recommendations (비즈니스 제언)
Dynamic Thresholding: Implement risk-based limits instead of static $5,000 rules.

Time-Based Sensitivity: Increase monitoring sensitivity during identified "Quiet Hours."

Behavioral Fingerprinting: Use V-feature correlations to flag accounts before the transfer is completed.

5. Technology Stack (기술 스택)
Language: Python 3.x

Environment: Google Colab

Libraries: Pandas, Seaborn, Matplotlib, OpenML
