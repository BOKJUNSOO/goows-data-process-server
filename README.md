# Goows data process platform!



[flink application repo](https://github.com/BOKJUNSOO/goows-flink-server)

[kafka application dev repo](https://github.com/BOKJUNSOO/goows-kafka-server)


# 디렉토리
`job` : `flink` submit 용 쉘파일이 위치한 디렉토리
`resource` : `flink` 어플리케이션의 `jar` 파일이 위치하는 디렉토리

- 클라우드 배포용 domain을 꼭 명시할것
```yaml
environment:
  - KAFKA_LISTENERS=PLAINTEXT://0.0.0.0:9092 # 내부 망
  - KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://CHANGE_THIS_URL_WITH_DOMAIN:9092 # 외부 망
```
