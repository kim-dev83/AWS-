Markdown
# 🚀 AWS 기반 웹 서비스 자동 배포 프로젝트

## 📌 프로젝트 소개
AWS 인프라를 활용하여 웹 서비스를 구축하고,  
Docker 및 CI/CD를 통해 자동 배포 환경을 구성한 프로젝트입니다.

👉 "클릭이 아닌 코드로 인프라를 구축하고 자동화까지 구현"

---

## 🏗️ 아키텍처

![architecture](./architecture/architecture.png)

### 📖 구성 설명
- **Route53** : 도메인 연결
- **ALB (Load Balancer)** : 트래픽 분산
- **EC2** : 웹 서버 운영
- **RDS** : 데이터베이스 관리
- **S3** : 정적 파일 저장
- **CloudWatch** : 모니터링

---

## ⚙️ 사용 기술

- AWS (EC2, RDS, S3, ALB)
- Docker
- GitHub Actions (CI/CD)
- Terraform (IaC)

---

## 🔄 CI/CD 흐름

1. GitHub 코드 push
2. GitHub Actions 실행
3. Docker 이미지 빌드
4. EC2 서버 자동 배포

---

## 🌐 실행 결과

👉 http://본인-서버-IP 또는 도메인

---

## 🛠️ 트러블슈팅

### ❗ 문제 1
EC2 접속 불가

- 원인 : 보안 그룹에서 SSH(22번 포트) 미허용
- 해결 : 포트 22 허용 후 정상 접속

---

### ❗ 문제 2
웹 페이지 접속 불가

- 원인 : Docker 포트 설정 오류
- 해결 : 포트 매핑 수정 (80:80)

---

## 📚 배운 점

- 클라우드 인프라 구조 설계 경험
- Docker 기반 배포 자동화 이해
- CI/CD 파이프라인 구축 경험

---

## 🙋‍♂️ 한 줄 요약

👉 "인프라 설계 + 자동화 + 운영 경험을 포함한 실무형 프로젝트"
