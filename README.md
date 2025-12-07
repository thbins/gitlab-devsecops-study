# GitLab CI/CD Practice

GitLab CI/CD와 보안 도구를 활용한 안전하고 빠른 파이프라인 구축 실습 프로젝트

![Architecture](./Architecture.png)

## 📁 프로젝트 구조

```
gitlab-ci-practice/
├── fundamental/          # GitLab CI/CD 기본 개념 실습
│   ├── gitlab/          # GitLab CI 기본 기능
│   └── tools/           # 보안 및 DevSecOps 도구
└── projects/            # 실전 프로젝트
    ├── 0. python/       # Python Flask 애플리케이션
    ├── 1. backend/      # Terraform 백엔드 인프라
    └── 2. app-gitops/   # GitOps 기반 배포 자동화
```

## 🎯 Fundamental - GitLab CI 기본 실습

### GitLab CI 핵심 기능

| 디렉토리 | 학습 내용 |
|---------|----------|
| **1. job practice** | 기본 작업 정의 및 스크립트 실행 |
| **2. default and variables practice** | 전역 설정 및 변수 관리 |
| **3. anchor and artifacts practice** | YAML 앵커 및 아티팩트 수집 |
| **4. aws integration** | OIDC 기반 AWS 인증 통합 |
| **5. rules** | 조건부 작업 실행 규칙 |
| **6. stages** | 파이프라인 스테이지 관리 |
| **7. caches** | 작업 간 캐시 공유 |
| **8. apprunner** | AWS App Runner 자동 배포 |

## 🔒 DevSecOps 도구 실습

### 보안 스캔 도구

| 도구 | 목적 | 주요 기능 |
|-----|------|----------|
| **Gitleaks** | 시크릿 탐지 | API 키, 토큰 등 민감정보 스캔 |
| **Semgrep** | SAST | 코드 보안 취약점 정적 분석 |
| **Trivy** | 컨테이너 보안 | 이미지 취약점, 설정 오류, 시크릿 스캔 |
| **Nuclei** | DAST | 동적 웹 애플리케이션 보안 테스트 |
| **Cosign** | 이미지 서명 | AWS KMS 기반 컨테이너 서명/검증 |

## 🚀 실전 프로젝트

### 0. Python Flask Application
- Flask 웹 애플리케이션
- Docker 컨테이너화
- 의존성 관리

### 1. Backend Infrastructure
- Terraform S3 백엔드 구성
- 원격 상태 파일 관리
- AWS 인프라 프로비저닝

### 2. App GitOps
- GitLab 프로젝트 자동 생성
- Terraform으로 GitOps 구현
- OIDC 기반 AWS 인증
- KMS 키 관리
- App Runner 배포 자동화

## 🛠️ 기술 스택

### CI/CD
- GitLab CI/CD
- Docker
- AWS App Runner

### 보안
- Gitleaks (Secret Scanning)
- Semgrep (SAST)
- Trivy (Container Security)
- Nuclei (DAST)
- Cosign (Image Signing)

### 인프라
- Terraform
- AWS (S3, ECR, App Runner, IAM, KMS)
- GitLab OIDC

### 애플리케이션
- Python 3.12
- Flask 3.0
- Alpine Linux

## 📋 사전 요구사항

- GitLab 계정
- AWS 계정
- Docker
- Terraform
- GitLab Runner (선택사항)

## 🔑 주요 기능

### 보안 중심 파이프라인
- 시크릿 스캔으로 민감정보 노출 방지
- SAST/DAST로 코드 및 런타임 보안 검증
- 컨테이너 이미지 취약점 스캔
- 디지털 서명으로 이미지 무결성 보장

### 자동화된 배포
- OIDC 기반 안전한 AWS 인증
- 조건부 파이프라인 실행
- GitOps 방식의 인프라 관리
- App Runner 자동 배포 및 모니터링

### 효율적인 파이프라인
- 캐시 활용으로 빌드 시간 단축
- 아티팩트 공유로 작업 간 데이터 전달
- 병렬 실행으로 처리 속도 향상

## 📝 라이선스

이 프로젝트는 학습 목적으로 제작되었습니다.
