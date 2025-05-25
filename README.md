<div align="center">
   <h1> Google + NEWS = Goows </h1>
   <h3> 실시간 사용자 데이터 처리 플랫폼 </h3>
   <h3> Flink & kafka Application</h3>
</div>

<img src='https://github.com/user-attachments/assets/2df303c1-1cad-4e7e-a9e5-f3fea8fcab4a'>


## 📢 프로젝트 소개


`#실시간 인기 검색어` `#검색키워드 추천` `#Streamming` `#kafka` `#Flink`

<br>

`sliding window` 를 구현하여 사용자들의 키워드를 특정 세션동안 집계하고 이를 바탕으로 실시간 인기 검색어 순위 기능을 제공합니다.<br>

사용자가 입력한 키워드와 이를 바탕으로 검색된 뉴스기사를 분석하여 사용자가 볼만한 다음 뉴스를 추천해줍니다.<br>



<br>

## 🏹 주요 기능 소개


### 🎯 `API 서버와의 독립성` (시스템 아키텍처)

아래의 아키텍처와 같이 서비스를 구성하여 각각의 기능을 세분화 하였습니다.

<img src='https://github.com/user-attachments/assets/afe57462-88a8-40c8-be67-6848472c58a5'>

- `React Server` : 클라이언트와 백엔드 서버간의 인터페이스 역할을 합니다.\
[프론트엔드 서버 레포는 여기!](https://github.com/Hwanjin-Choi/project-goose-frontend)

- `Spring Server` : `API` 요청에 대한 응답을 전문적으로 담당합니다.\
[백엔드 스프링 서버 레포는 여기!](https://github.com/SoonWookHwang/goows)

- `Flink & Kafka Server` : 실시간 데이터 집계, 추천 기능등 데이터 처리를 전문적으로 담당합니다.\
[실시간 데이터 처리 플랫폼은 여기!](https://github.com/BOKJUNSOO/goows-data-process-server)\
[goows Flink 어플리케이션 소스코드 레포는 여기!](https://github.com/BOKJUNSOO/goows-flink-server)\
[Kafka 개발환경 레포는 여기!](https://github.com/BOKJUNSOO/goows-kafka-server)

<br>

### 🎯 `실시간 인기 검색어 순위`
사용자가 입력으로 주어진 키워드 `각각`이 `3분`이라는 세션을 가지며\
실시간으로 집계되어 `단위시간 내`의 인기 키워드를 확인할 수 있습니다.


<br>
<img width="1000" alt="trendingKeyword" src="https://github.com/user-attachments/assets/0de4fcda-2369-44ff-b160-53a01ed2be6d">
<br>

<br>

### 🎯 `검색어 추천 기능`
특정 키워드 검색 이후 연관된 기사를 검색할 수 있도록\
연관 검색어 추천 기능을 구현했습니다.<br>

이 기능은은 간소화된 `UI`의 한계를 극복하고, 다양한 정보에 접근 할 수 있도록 합니다.

<br>
<img width="1000" alt="recommand" src="https://github.com/user-attachments/assets/6caf26ce-3cdd-4275-b73c-79be9d04c8ff">
<br>

<br>

## ⚒️ 기술 스택
| 분류 | 기술 |
| ---- | ---- |
| 언어 | <img src="https://img.shields.io/badge/OpenJDK-11-007396?style=flat-square&logo=openjdk&logoColor=white" />|
| 프레임워크/플랫폼 |<img src="https://img.shields.io/badge/Flink-1.17.1-E6526F?style=flat-square&logo=apache-flink&logoColor=white" /> <img src="https://img.shields.io/badge/Kafka-Latest-231F20?style=flat-square&logo=apache-kafka&logoColor=white" />|
| 사용 라이브러리 | <img src="https://img.shields.io/badge/KOMORAN-3.3.9-blue?style=flat-square&logo=komoran&logoColor=white">|
| 배포 |  <img src="https://img.shields.io/badge/GCP-Google_Cloud_Platform-4285F4?style=flat-square&logo=google-cloud&logoColor=white" /> <img src= "https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"> |

<br>

## 🏆 goows 팀원 깃허브

<table align="center" width="100%">
  <tr>
    <td><img src="https://avatars.githubusercontent.com/u/170910509?v=4"/></td>
    <td><img src="https://avatars.githubusercontent.com/u/206484294?v=4"/></td>
    <td><img src="https://avatars.githubusercontent.com/u/68840464?v=4"/></td>
    <td><img src="https://avatars.githubusercontent.com/u/204177408?v=4"/></td>
    <td><img src="https://avatars.githubusercontent.com/u/170912062?v=4"/></td>
    <td><img src="https://avatars.githubusercontent.com/u/108779266?v=4"/></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/Lookies09">김형균</a>
    </td>
    <td align="center"><a href="https://github.com/DDu-DDu">이민기</a>
    </td>
    <td align="center"><a href="https://github.com/Hwanjin-Choi">최환진</a>
    </td>
    <td align="center"><a href="https://github.com/Dingcobel">김민지</a>
    </td>
    <td align="center"><a href="https://github.com/BOKJUNSOO">복준수</a>
    </td>
    <td align="center"><a href="https://github.com/SoonWookHwang">황순욱</a>
    </td>
  </tr>
  <tr>
    <td align="center">FrontEnd</td>
    <td align="center">FrontEnd</td>
    <td align="center">FrontEnd</td>
    <td align="center">BackEnd</td>
    <td align="center">BackEnd</td>
    <td align="center">BackEnd</td>
  </tr>
</table>

<br>



## 🔥 Data Engineering 에서의 도전 과제

`뉴스` 라는 도메인이 정해졌고, 이를 바탕으로 서비스를 만들어내는 과정에서 다음과 같은 사항이 고려되어야 했습니다.

- 어떤 기능이 있다면 서비스가 `차별성`이 존재할 것인가?

- 해당 기능을 구현하기 위해서 데이터가 `어떻게 처리`되어야 하는가?

- 해당 기능을 구현하기 위해서는 `어떤 프레임워크`를 사용할 것인가 ?



```
세부적인 내용은 아래 링크의 velog에서 확인할 수 있습니다!
(작성중..)
```

1. 무엇을 구현할까\
[실시간 인기검색어 순위와 추천 키워드 기능](www.naver.com)


2. 어떻게, 그리고 왜 그렇게 구현할까?\
[Stream vs Batch](www.naver.com)\
[Flink & Kafka](www.naver.com)


<br>

## 🫡 deploy

- [flink application repo](https://github.com/BOKJUNSOO/goows-flink-server) 소스코드를 이용하여 빌드한 `jar`을 준비합니다.\
(해당 레포의 README 참고)


- `resource` 디렉토리 해당 파일을 위치시킵니다.

- 클라우드 배포용 domain을 꼭 명시합니다.
```yaml
environment:
  - KAFKA_LISTENERS=PLAINTEXT://0.0.0.0:9092 # 내부 망
  - KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://CHANGE_THIS_URL_WITH_DOMAIN:9092 # 외부 망
```

<br>

- `docker` 버전에 맞추어 컨테이너를 빌드합니다.
```bash
sudo docker compose up -d
```

<br>

- `job` : `flink` submit 용 쉘파일을 컨테이너 내부에서 실행 시킵니다.
```bash
sudo docker exec -it <user_jobmanager_container_name> /bin/bash
```

- `/opt/flink/job` 디렉토리에서 쉘파일을 이용해 `job`을 제출합니다.
```bash
# in /opt/flink/job directory
./submit.sh

# 권한문제가 생긴다면
chmod 777 ./submit.sh
```


