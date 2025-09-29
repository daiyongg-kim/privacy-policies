# Privacy Policies for Apps

이 프로젝트는 GitHub Pages를 활용하여 여러 앱의 개인정보처리방침을 한 곳에서 관리하는 시스템입니다.

## 🌐 URL 구조

- **메인 페이지**: `https://yourusername.github.io/privacy-policies/`
- **앱별 개인정보처리방침**: `https://yourusername.github.io/privacy-policies/[app-name]/`

## 📁 프로젝트 구조

```
privacy-policies/
├── index.html              # 메인 페이지 (앱 목록)
├── css/
│   └── style.css           # 공통 스타일
├── the-daily-utils/
│   └── index.html          # The Daily Utils 개인정보처리방침
├── [other-app-name]/
│   └── index.html          # 다른 앱의 개인정보처리방침
└── README.md
```

## 🚀 GitHub Pages 설정 방법

### 1단계: GitHub 저장소 생성 및 설정

1. **GitHub에서 새 저장소 생성**:
   - Repository name: `privacy-policies` (또는 원하는 이름)
   - Public으로 설정 (GitHub Pages 무료 사용을 위해)
   - README.md 포함하지 않음 (이미 존재)

2. **로컬에서 Git 초기화 및 연결**:
   ```bash
   # 프로젝트 디렉토리로 이동
   cd privacy-policies-project

   # Git 초기화 (아직 안 했다면)
   git init

   # 모든 파일 추가
   git add .

   # 첫 번째 커밋
   git commit -m "Initial privacy policies setup with multi-language support"

   # 메인 브랜치로 변경
   git branch -M main

   # GitHub 저장소 연결
   git remote add origin https://github.com/daiyongg-kim/privacy-policies.git

   # 저장소에 푸시
   git push -u origin main
   ```

### 2단계: GitHub Pages 활성화

1. **GitHub 저장소로 이동**:
   - `https://github.com/daiyongg-kim/privacy-policies`

2. **Settings 탭 클릭**

3. **Pages 메뉴로 이동** (좌측 사이드바에서)

4. **Source 설정**:
   - "Deploy from a branch" 선택
   - Branch: `main` 선택
   - Folder: `/ (root)` 선택
   - Save 버튼 클릭

### 3단계: 배포 확인

1. **배포 상태 확인**:
   - Actions 탭에서 배포 진행 상황 확인
   - 초록색 체크마크가 나타나면 배포 완료

2. **웹사이트 접속**:
   - 5-10분 후 `https://daiyongg-kim.github.io/privacy-policies/` 접속 가능
   - The Daily Utils 개인정보처리방침: `https://daiyongg-kim.github.io/privacy-policies/the-daily-utils/`

### 4단계: Play Console에서 사용

Google Play Console > 정책 > 개인정보처리방침 URL에 입력:

```
https://daiyongg-kim.github.io/privacy-policies/the-daily-utils/
```

### 5단계: 사용자 정의 도메인 설정 (선택사항)

1. **도메인 소유 시**:
   - GitHub Pages Settings에서 Custom domain 설정
   - DNS에서 CNAME 레코드를 daiyongg-kim.github.io로 설정

2. **HTTPS 강제 활성화**:
   - "Enforce HTTPS" 체크박스 활성화

### 문제 해결

**배포가 안 될 때**:
- Actions 탭에서 오류 메시지 확인
- 파일 권한 및 구조 검토
- 브랜치 이름이 올바른지 확인

**404 오류가 날 때**:
- 5-10분 대기 (DNS 전파 시간)
- 브라우저 캐시 삭제
- URL 경로가 올바른지 확인

## 📱 새 앱 추가하는 방법

1. **새 폴더 생성**: `new-app-name/`
2. **index.html 파일 생성**: 개인정보처리방침 내용 작성
3. **메인 index.html에 앱 추가**: 앱 목록에 새 앱 링크 추가
4. **커밋 및 푸시**: GitHub에 업로드하면 자동으로 페이지 업데이트

## 🔗 Play Console에서 사용법

Google Play Console > 정책 > 개인정보처리방침 URL에 다음과 같이 입력:

```
https://daiyongg-kim.github.io/privacy-policies/the-daily-utils/
```

## ✨ 특징

- **무료 호스팅**: GitHub Pages 무료 사용
- **자동 배포**: 코드 푸시하면 자동으로 웹사이트 업데이트
- **반응형 디자인**: 모바일, 태블릿, 데스크톱 지원
- **다국어 지원**: 각 앱별로 다국어 페이지 생성 가능
- **SEO 최적화**: 검색 엔진 최적화 적용
- **HTTPS 지원**: 기본적으로 HTTPS 제공

## 📋 관리 팁

1. **버전 관리**: Git을 통한 변경 이력 추적
2. **백업**: GitHub에 자동 백업
3. **협업**: 팀원과 함께 관리 가능
4. **템플릿 활용**: 새 앱 추가 시 기존 구조 복사