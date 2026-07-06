# 이미지 위젯 (노션 임베드용)

이미지를 올리면 hover 확대 효과가 있는 위젯이 만들어지고, 클릭하면 지정한 링크로 이동합니다.

## 사용법

1. **관리 페이지 열기**: `https://kjm9954.github.io/image-widget/admin.html`
2. GitHub Personal Access Token 저장 (최초 1회, repo 권한 필요)
3. 이미지를 끌어다 놓고 → 링크 URL 입력 → **GitHub에 올리기**
4. 만들어진 임베드 URL을 노션에서 `/embed` 로 붙여넣기

## 위젯 기능

- 마우스 hover 시 서서히 확대 (scale 1.06)
- 클릭 시 지정 링크 새 탭으로 이동
- 위젯 **오른쪽 상단 모서리** 클릭 → ⚙ 설정 버튼 표시 → URL 즉석 변경

## 토큰 발급

GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
→ `repo` 권한 체크 후 생성. 토큰은 이 기기 브라우저(localStorage)에만 저장됩니다.

## 파일 구성

- `admin.html` — 이미지 업로드/관리 페이지
- `index.html` — 위젯 본체 (`?id=위젯ID`)
- `widgets.json` — 위젯 목록 데이터
- `images/` — 업로드된 이미지
