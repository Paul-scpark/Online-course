# ETL and Data Pipelines with Shell, Airflow and Kafka (IBM) 5주차

이번 글에서는 [Coursera의 ETL and Data Pipelines with Shell, Airflow and Kafka (IBM)](https://www.coursera.org/learn/etl-and-data-pipelines-shell-airflow-kafka/home/info) 5주차 강의를 정리합니다. <br/>
이 강좌는 ETL 및 ELT 데이터 파이프라인에 대해 학습하며, Airflow와 Kafka 등을 이용해 이를 배우게 됩니다. <br/>
5주차에는 `지금까지 배운 내용들에 대한 파이널 프로젝트`에 대해 공부합니다.

---

## 1. 프로젝트에 대한 개요
- ETL을 수행하고, 파이프라인을 만들어서 데이터를 DB에 업로드
- 실습에서는 Airflow와 Kafka를 모두 사용
- 도로 교통 데이터를 분석하여 국도의 정체를 해소하는 것을 목표로 하는 프로젝트
  - 각 고속도로는 서로 다른 파일 형식을 사용하고 있음
  - 따라서 다양한 형식으로 사용 가능한 데이터를 수집 및 단일 파일로 통합해보기
  - 차량이 톨게이트를 통과하면, `vehicle_id, vehicle_type, toll_plaza_id` 및 타임스탬프와 같은 차량 데이터가 kafka로 스트리밍
  - 이 스트리밍 데이터를 수집하여 데이터베이스에 로드하는 데이터 파이프라인을 생성해보기

## 2. 프로젝트 채점 기준
- 작업 1: DAG 인수 정의, DAG 정의, 데이터 다운로드 작업, csv 및 tsv 파일에서 데이터 추출, 고정 너비 파일에서 데이터 추출, 이전 작업에서 추출한 데이터 통합 및 변환, 작업 파이프라인 정의, DAG 제출, DAY 일시 중지 해제, DAG 모니터링
- 작업 2: Zookeeper 시작, Kafka 서버 시작, toll 이라는 주제 만들기, 유료 교통 시뮬레이터 다운로드 & 구성 & 실행, streaming_data_reader.py 구성 및 실행, 스트리밍 데이터 파이프라인 상태 확인
- 각 작업은 스크린샷을 통해서 제출할 것

## 3. Final Assignment (Part 1)
> Creating ETL Data Pipeline Using Apache Airflow

- IBM에서 제공하는 Lab 환경에서 실행합니다.

## 4. Final Assignment (Part 2)
> Creating Streaming Data Pipelines Using Kafka

- IBM에서 제공하는 Lab 환경에서 실행합니다.
