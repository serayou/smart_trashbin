# 스마트 쓰레기통 관리 시스템

스마트 디바이스 프로그래밍, 19년 여름 프로젝트

**적재량 감지센서**를 이용하여 쓰레기통의 적재 현황을 모니터링 할 수 있습니다.
적재 현황과 비상 상황 알림을 통해 쓰레기통이 넘치는 상황과 쓰레기통이 넘어지는 등의 예기치 못한 상황을 방지하여  공공장소의 청결도를 향상시킬 수 있습니다.

## 환경

Cortex-M3 Processor 3대, Raspberry pi 1대, Server 용 PC

## 사용방법
#### Server
1. [mosquitto](https://mosquitto.org/download/) 설치
2. 브로커 실행 ```mosquitto -v``` 
  > *참고*
  > * mosquitto broker : ```mosquitto -v```
  > * mosquitto subscribe : ```mosquitto_sub -t topic```
  > * mosquitto publish : ```mosquitto_pub -t topic -m "msg"```


#### Client
1. [Tera Term](https://ttssh2.osdn.jp/index.html.en) 설치
2. 보드 연결 후, Tera Term 실행 및 보드 RST 키 입력
3. ALT+F,T,Y,S 하여 client의 bin 파일 올리기 (Debug>Exe에 존재)
  
## 정보
