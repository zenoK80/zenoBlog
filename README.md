# zenoBlog

Laravel + Tailwind CSS 로 구현하는 개인 블로그 서비스

---

## 프로젝트 소개

**zenoBlog** 는 Laravel 프레임워크와 Tailwind CSS 를 활용해 개발하는 개인 블로그 서비스입니다.

- 포트폴리오 목적 + 실제 서비스 운영 목적
- 로그인 후 에디터로 글 작성 / 수정 / 삭제
- 댓글, 조회수 통계, URL 공유 기능

---

## 기술 스택

| 분류 | 기술 | 설명 |
|------|------|------|
| Backend | Laravel 11 | PHP 프레임워크 |
| Frontend | Tailwind CSS | 유틸리티 CSS 프레임워크 |
| Frontend | Alpine.js | 경량 JS 인터랙션 |
| Editor | Toast UI Editor | 마크다운 에디터 |
| Server | Apache (MAMP) | 로컬 개발 서버 |
| DB | MySQL | 데이터베이스 |
| VCS | Git / GitHub | 버전 관리 |

---

## 로컬 실행 환경

```
프로그램: MAMP
PHP: 8.3.1
접속 URL: http://127.0.0.1:8000
프로젝트 경로: D:\develop\0_zeno\laravel\zenoBlog
```

---

## 로컬 실행 방법

```bash
# 프로젝트 클론
git clone https://github.com/zenoK80/zenoBlog.git

# 디렉토리 이동
cd zenoBlog

# 패키지 설치
composer install
npm install

# 환경 설정
cp .env.example .env
php artisan key:generate

# DB 마이그레이션
php artisan migrate

# 개발 서버 실행
php artisan serve
npm run dev
```

---

## 폴더 구조

```
zenoBlog/
│
├── app/
│   ├── Http/
│   │   └── Controllers/       ← 요청 처리
│   └── Models/                ← DB 모델
│
├── config/                    ← Laravel 설정 파일
│
├── database/
│   └── migrations/            ← 테이블 생성 파일
│
├── public/                    ← 웹 진입점
│
├── resources/
│   ├── css/                   ← Tailwind CSS
│   ├── js/                    ← JavaScript
│   └── views/                 ← Blade 템플릿
│
├── routes/
│   └── web.php                ← URL 라우팅
│
└── .env                       ← 환경 변수 (DB 접속 정보 등)
```

---

## 주요 기능

- [ ] 로그인 / 회원가입
- [ ] 글 작성 / 수정 / 삭제
- [ ] 마크다운 에디터 연동
- [ ] 이미지 업로드
- [ ] 댓글
- [ ] 조회수 / 통계
- [ ] URL 공유 / OG 태그
- [ ] 관리자 페이지
- [ ] 배포

---

## GitHub

[https://github.com/zenoK80/zenoBlog](https://github.com/zenoK80/zenoBlog)
