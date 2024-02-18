# AWS 콘솔을 활용한 3tier 구축

### 목표 아키텍쳐
![image](https://github.com/plum-king/3tier-AWS-console/assets/77599304/0758c6ca-a4a5-4899-b6dc-edc8b33d485d)

### 일정표
|주제|날짜|태그|
|:---:|:---:|:---:|
|IAM 설정|2024.01.17|`Identity Center` `IAM`|
|아키텍쳐 완성 및 네트워크 구성|2024.01.19|`VPC` `RT` `IGW` `SG`|
|가용영역 A 구성|2024.01.20-21|`Tomcat` `Apache`|
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

### Settings
**1. IAM 설정 (1/17)**
  - [IAM Identity Center로 그룹 및 사용자 생성](https://plum-king.tistory.com/25)
  - [IAM 그룹 권한 추가하기](https://plum-king.tistory.com/26)
  - 추가: [IAM 기본 사용자 생성하기](https://plum-king.tistory.com/27)
**2. 네트워크 구성 (1/19)**
**3. Bastion Host 생성 (1/19)**

### 가용영역 A 설정
**1. WEB-A 서버 생성 (1/19)**
**2. Bastion → WEB-A 접근 (1/19-20)**
**3. WEB-A 세팅 (1/20)**
**4. WAS-A 서버 생성 (1/20)**
**5. Bastion → WAS-A 접근 (1/20)**
**6. WAS-A 세팅 (1/20)**
**7. WEB-A ↔ WAS-A 연결 (1/20-21)**

### DB 생성 및 설정
**1. RDS 생성 및 설정 (1/21-22)**
**2. WAS ↔ RDS 연결 (1/22)**
**3. WEB ↔ WAS ↔ DB 연결 확인 (1/22)**

### LB
**1. In-WAS-ALB 생성 및 설정 (1/22)**
**2. In-WAS-ALB 연결 확인 (1/22)**
**3. Ex-WEB-ALB 생성 및 설정 (1/22)**

### AMI 생성 및 AutoScaling
**1. AMI 및 시작 템플릿 생성 (1/22)**
**2. Auto Scaling 그룹 생성 (1/22)**
**3. WAS LB 확인 (1/23)**
**4. ALB↔AS 라운드 로빈 테스트 (1/22-23)**
**5. Auto Scaling 부하 테스트 (1/23)**

### Route53
**1. 도메인 생성 및 Route53 연결 (1/22)**
**2. ACM 인증서 생성 (1/22)**
**3. HTTPS 연결 (1/22)**

### Trouble Shooting
**1. scp 트러블 슈팅 (1/20)**
**2. Bastion → WEB 트러블 슈팅 (1/20)**
**3. Tomcat 접근 트러블슈팅 (1/20-21)**
**4. WEB 접속 트러블슈팅 (1/21)**
**5. Tomcat 부팅 시 안켜짐 (1/21)**
**6. WAS에서 dbtest.jsp 접속 불가 (1/22)**
**7. DB 연결 확인 불가 (1/22)**
**8. 대상그룹 UnHealthy 상태 (1/23)**
**9.WAS-C 무한대 생성 오류 (1/23)**

### 회고

