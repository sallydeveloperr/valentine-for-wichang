<img src="https://capsule-render.vercel.app/api?type=waving&color=ff69b4&height=180&section=header&text=💝발렌타인데이%20선물%20웹페이지💝&fontSize=42&fontColor=ffffff" />

발렌타인데이를 맞아 특별한 사람을 위해 만든 인터랙티브 웹 선물입니다.

## 📌 프로젝트 소개

이 프로젝트는 발렌타인데이를 축하하기 위한 웹 기반 인터랙티브 선물입니다. 편지 열기부터 퀴즈, 쿠폰까지 다양한 단계로 구성되어 있으며, 사용자에게 즐거운 경험을 선사합니다!

## ✨ 주요 기능

### 1. 편지 오픈 애니메이션
- 클릭으로 편지봉투를 여는 인터랙티브 애니메이션
- 하트가 떨어지는 시각 효과

### 2. Yes/No 버튼 게임
- "Will you be my Valentine?" 질문
- Yes 버튼은 점점 커지고, No 버튼은 도망가는 재미있는 인터랙션
- 고양이 이미지가 함께 등장하는 귀여운 UI

### 3. 퀴즈 타임
총 3개의 커플 맞춤 퀴즈:
- 첫 만남일
- 연애 시작일
- 내가 좋아하는 초콜릿!

정답을 맞추면 축하 애니메이션과 함께 다음 문제로 진행됩니다.

### 4. 스페셜 쿠폰
- 퀴즈를 모두 맞추면 받을 수 있는 특별 쿠폰
- 바코드가 포함된 실제 쿠폰 디자인
- PNG 이미지로 다운로드 가능 (16:9 비율)

### 5. 최종 편지
- 타이핑 효과가 있는 마지막 메시지
- 지속적으로 떨어지는 하트 애니메이션

## 🎨 디자인 특징

- **색상 테마**: 핑크 그라데이션 (#ffeef8 → #ffe8f5 → #ffd4ed)
- **폰트**: Gamja Flower (구글 폰트)
- **모바일 최적화**: 반응형 디자인, iOS Safe Area 지원
- **애니메이션**: 
  - 페이드인 전환 효과
  - 하트 떨어지는 애니메이션
  - 정답 시 폭죽/이모지 버스트 효과
  - 토스트 메시지

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: 
  - Flexbox 레이아웃
  - CSS 애니메이션 & Keyframes
  - 그라데이션 & 그림자 효과
- **JavaScript (Vanilla JS)**:
  - DOM 조작
  - 이벤트 핸들링
  - 동적 애니메이션 생성
- **외부 라이브러리**:
  - [html2canvas](https://html2canvas.hertzen.com/): 쿠폰 이미지 다운로드 기능

## 📱 모바일 지원

- iOS 및 Android 완벽 지원
- Safe Area Inset 적용 (노치 디자인 대응)
- Touch 이벤트 최적화
- 뷰포트 스케일 고정 (확대/축소 방지)

## 🚀 사용 방법

1. **파일 다운로드**
   ```bash
   git clone https://github.com/yourusername/valentine-gift.git
   cd valentine-gift
   ```

2. **브라우저에서 열기**
   - `index.html` 파일을 더블클릭하거나
   - 웹 서버를 통해 실행 (권장)
   ```bash
   # Python 간단한 웹서버 실행
   python -m http.server 8000
   ```
   - 브라우저에서 `http://localhost:8000` 접속

3. **GitHub Pages로 배포** (선택사항)
   - GitHub Repository 설정 → Pages
   - Source: main 브랜치 선택
   - 몇 분 후 `https://yourusername.github.io/valentine-gift/` 에서 접근 가능

## 📂 프로젝트 구조

```
valentine-gift/
│
├── index.html          # 메인 HTML 파일 (모든 코드 포함)
├── README.md           # 프로젝트 설명서
│
└── assets/             # (선택) 이미지/GIF 파일
    ├── cat_dance.gif   # 고양이 댄스 GIF
    └── cat_heart.gif   # 하트 든 고양이 GIF
```

## 🎯 커스터마이징 가이드

### 퀴즈 내용 변경
`index.html` 파일의 `quiz` 배열을 수정하세요:

```javascript
const quiz = [
    {
        question: "당신의 질문",
        options: ["선택지1", "선택지2", "선택지3", "선택지4"],
        correct: 0,  // 정답 인덱스 (0부터 시작)
        message: "정답 메시지"
    },
    // ... 더 추가
];
```

### 색상 테마 변경
CSS의 다음 부분을 수정하세요:

```css
body {
    background: linear-gradient(135deg, #ffeef8 0%, #ffe8f5 50%, #ffd4ed 100%);
}

h1 {
    color: #ff69b4;
}
```

### 쿠폰 혜택 변경
`couponScreen` 섹션의 HTML 내용을 수정하세요.

## 🐛 알려진 이슈

- GIF 파일 경로가 상대경로로 되어 있어, 같은 폴더에 `cat_dance.gif`, `cat_heart.gif` 파일이 필요합니다.
- html2canvas 라이브러리는 CDN에서 로드되므로 인터넷 연결이 필요합니다.

## 📝 라이선스

이 프로젝트는 개인 선물용으로 제작되었습니다.

## 💌 제작자

- **제작**: Sallychoe
- **제작일**: 2025년 2월
- **목적**: 발렌타인데이 선물

---

Made with 💖 for Valentine's Day 2026
