## HELIOS: Federated Learning Platform
HELIOS는 AI 진단기술의 접근성이 떨어지는 중소 병원 및 지역병원을 위한 AI 기반 연합 학습(Federated Learning)을 웹상에서 제공하는 플랫폼입니다. 

### 🛠 Tech Stack
- Frontend: React (Vite), Nginx
- Backend: Spring Boot 3, Java 21, JPA/Hibernate 
- AI/ML: Python, Websockets, aiohttp
- Database: PostgreSQL 15
- Infrastructure: Docker, Docker Compose, Cloud

### ⚡ Quick Start (Docker)
Docker을 설치해야함

# 1. 메인 레포 클론
```
git clone https://github.com/Helios-G/HELIOS-Main.git
cd HELIOS-Main
```

# 2. 클론한 메인레포 내에서 각 서비스 레포 클론
-git clone https://github.com/Helios-G/helios_backend.git
-git clone https://github.com/Helios-G/Heliosclient.git
-git clone https://github.com/Helios-G/helios_ai.git

# 3. 실행
```
docker-compose up --build
```

개별 서비스 접속 주소
- Frontend: http://localhost:3000
- Backend API: http://localhost:8081
- AI Server: ws://localhost:8083

### 📂 Project Structure
helios_backend: Spring Boot 기반의 비즈니스 로직을 처리하는 메인 서버
helios_ai: 연합 학습 처리를 위한 파이썬 서버 
Heliosclient: 사용자 인터페이스를 제공하는 웹 프론트엔드

### 👥 Contributors
김다인 ( ) : Backend & Infrastructure
오예진 ( ) : Backend & Database
김선민 ( ) : Frontend & Federated Learning
최효빈 ( ) : Labeling & Federated Learning
