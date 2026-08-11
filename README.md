# Seungbin Yang — Personal Homepage

Jon Barron 계열의 미니멀 아카데믹 스타일 개인 홈페이지 (단일 `index.html`, 빌드 도구 불필요).

## 배포 방법 (GitHub Pages)

1. GitHub에서 **`<내아이디>.github.io`** 라는 이름의 public 저장소를 새로 만든다.
2. 이 폴더의 내용물(`index.html`, `assets/`)을 저장소 루트에 push 한다:

   ```bash
   cd homepage
   git init
   git add index.html assets README.md
   git commit -m "Initial homepage"
   git remote add origin git@github.com:<내아이디>/<내아이디>.github.io.git
   git push -u origin main
   ```

3. 몇 분 뒤 `https://<내아이디>.github.io` 에서 접속 확인.
   (Settings → Pages 에서 Source가 `main` 브랜치인지 확인)

## 배포 전 직접 채워야 하는 것

- [x] **프로필 사진**: `assets/profile.jpg` 적용 완료 (증명사진 정사각 크롭, 400px)
- [x] **GitHub 링크**: https://github.com/sbY99 적용 완료
- [x] **News 날짜 확인 완료**: ICLR 2026 억셉 통보 2026-01-25(공식 발표),
      ACL 2026 억셉 통보 2026-04-04(공식 사이트 important dates) — 페이지에 Jan/Apr 2026으로 반영됨

참고: CV PDF는 공개하지 않기로 하여 사이트에서 제외됨 (아이콘·파일 삭제).

## 내용 수정

모든 내용은 `index.html` 하나에 있고 섹션 순서대로 배치되어 있다:
헤더(소개/아이콘 링크) → News → Publications → Experience → Education.

- 논문 추가: `Publications` 섹션의 `<div class="pub">` 블록 하나를 복사해서 수정
- 본인 이름 강조는 `<span class="me">Seungbin Yang</span>`, 동등기여는 `*`
- 다크 모드는 방문자 OS 설정에 따라 자동 적용됨 (별도 작업 불필요)
