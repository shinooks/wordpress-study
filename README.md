# 워드프레스 활용 시스템 고도화 프로젝트

## 프로젝트 팀 명: 유자치즈케익

| 구성원 |  |
| --- | --- |
| 정동영 | 이준범 |
| 박태준 | 신승민 |
| 김태윤 | 황신욱 |

## 프로젝트 링크
- [노션 공개페이지](https://www.notion.so/Wordpress-1de07373030f80e085f7e443927178f7)
- 프로젝트 원본 링크
  - 퍼블릭: [3조 유자치즈케익](https://www.notion.so/3-1dc13e81f3ba80b0b0b1deb07cdc68c4?pvs=21) 
  - 노션 개인페이지: [3조 유자치즈케익](https://www.notion.so/3-1dc13e81f3ba80b0b0b1deb07cdc68c4?pvs=21)  


## 1. 프로젝트 개요

<aside>
**💡 Wordpress를 활용하여 시스템 설계 방법에 대해 학습하고 점진적으로 고도화 하는 프로젝트**
</aside>

## 2. 프로젝트 진행 방식

1. 매일 시스템의 목표를 설정해 스터디
    - 단일 서버부터 2티어 구조, 3티어 구조, 고가용성 구조 등
    - 현재 단계의 한계점을 나누고 다음 시스템 목표로 설정
2. 각자 시스템을 직접 구현하고 코드 기반으로 재구현이 가능한 방식으로 결과물 구성
    - 기술 스택을 Vagrant와 Virtualbox, Shell Script로 통일
3. 프로젝트 진행 과정을 문서화
    - 자신이 현재까지 구현한 단계, 구현 방법, 그 과정에서 만난 문제를 매일 기록
4. 프로젝트 진행 과정을 팀과 교환
    - 당일 6시부터는 자신이 진행한 프로젝트 진행 사항 및 결과를 구성원들과 교환

---

## 3. 프로젝트 아키텍처 목표

- 이 프로젝트는 WordPress를 기반으로 한 웹 시스템을 **처음부터 고도화하는 과정**을 실습합니다.
- 실무에서 필요한 **확장성, 안정성, 관리 효율성**을 고려한 시스템을 직접 설계하고 만들어보는 것이 목표
- 단순한 설치에서 시작해, 점점 더 실제 운영 환경에 가까운 구조로 발전시키며, 각 단계마다 **왜 이런 구성이 필요한지를 생각해보기**.

### 1. 단일서버 아키텍처 구성

![image](https://github.com/user-attachments/assets/c2112ef1-8e75-4d3e-8644-7224e8c3c0a4)

### 2. 2-Tier 아키텍처 구성

![image](https://github.com/user-attachments/assets/6df9be39-04b2-4eb0-8f6c-b94f72a2465f)


### 3. 3-Tier 아키텍처 구성

![image](https://github.com/user-attachments/assets/ab3eebe1-b23a-4046-91ac-3f9143753a74)


### 4. NFS로 다수의 Wordpress 환경에서 설정 동기화

![image](https://github.com/user-attachments/assets/69ab9a21-34d6-4d04-a910-6778c464cc41)


### 5. iSCSI로 MySQL의 데이터를 분산 스토리지에 저장

![image](https://github.com/user-attachments/assets/a8b077cc-b8d5-4521-9af9-0b70874efd27)


### 6. MySQL의 빠른 복구를 위한 데이터베이스 레플리케이션 구성

![image](https://github.com/user-attachments/assets/3b384b00-180e-48cf-bf36-e7004f0942a3)
