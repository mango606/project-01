# Gitlab을 사용한 CI/CD 실습

> ✅ CI와 CD의 정의와 목적을 이해한다.<br>
> ✅ CI/CD를 도입함으로써 얻을 수 있는 장점을 학습한다.<br>
> ✅ GitLab의 설정 파일 작성 방법을 익히고, 이를 활용하여 자동화된 빌드 및 배포 파이프라인을 구축한다.<br>
> ✅ AWS와 같은 클라우드 플랫폼을 이용하여 CI/CD 파이프라인의 배포 단계를 자동화하는 방법을 학습한다.


## Amazon ECS

- **AWS Elastic Container Service**: docker 애플리케이션을 쉽게 배포하고 운영 할 수 있도록 지원하는 완전관리형 Container Orchestration 서비스
- AWS ECS는 크게 ECR, ECS Cluster, ECS Service, ECS Task로 이루어진다.

<p align="center">
  <img src="https://github.com/user-attachments/assets/2f1731d1-ff91-42a2-8e2d-86c655731631">
</p>


## AWS 설정
| 🛡️ AWS 보안 그룹                                                                            | 🏗️ AWS ECR                                                                                             |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| ![보안그룹](https://github.com/user-attachments/assets/1e800c08-d8ce-485f-bff3-fe6cf2559dd8) | ![프라이빗 리포지토리](https://github.com/user-attachments/assets/09dd77db-ca06-4c7b-a7e9-b94659f4943b)|

| 🚀 AWS ECS                                                                                  | 🔑 AWS IAM                                                                                             |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| ![클러스터](https://github.com/user-attachments/assets/3601aa82-f499-49cb-8d32-fe728bdce9c2) | ![사용자](https://github.com/user-attachments/assets/a90ae459-86af-48d8-ae22-2f24110d80cb)        |


## GitLab CI/CD 파이프라인 실행 과정

### 1️⃣ GitLab Pipelines 실행 및 스테이지 통과
<p align="center">
  <img src="https://github.com/user-attachments/assets/deb9f404-be82-4ddf-961c-68cd7b2522dc" width="700">
</p>

### 2️⃣ 컨테이너가 ECS에 반영됨
<p align="center">
  <img src="https://github.com/user-attachments/assets/d7c14fd7-a57e-42ed-a338-f3d270af85f0" width="700">
</p>
