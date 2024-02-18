# AWS 콘솔을 활용한 3tier 구축

### 일정표
|주제|날짜|태그|
|:---:|:---:|:---:|
|IAM 설정|2024.01.17|`Identity Center` `IAM`|
|아키텍쳐 완성 및 네트워크 구성|2024.01.19|`VPC` `RT` `IGW` `SG`|
|가용영역 A 구성|2024.01.20~21|`Tomcat` `Apache`|
|DB 생성 및 설정|2024.01.22|`RDS` `MySQL`|
|LB 구성 및 도메인 연결|2024.01.22|`LB` `TG` `Route53` `ACM`|
|Auto Scaling|2024.01.23|`Auto Scaling` `CloudWatch`|
|아키텍쳐 draw.io로 재구성|2024.01.23|`Architecture`|
|회고|2024.01.24|`Retrospect/회고`|

### IP 정보
|EC2 이름|프라이빗 IP|
|:---:|:---:|
|Bastion|10.101.1.214|
|WEB-A|10.101.2.195|
|WAS-A|10.101.3.5|

### 목표 아키텍쳐
![image](https://github.com/plum-king/3tier-AWS-console/assets/77599304/0758c6ca-a4a5-4899-b6dc-edc8b33d485d)
