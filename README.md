# hayoung.work

GitHub Pages(Jekyll) 기반 블로그.

## 새 글 쓰는 법

1. `_posts/` 폴더에 `YYYY-MM-DD-제목.md` 파일 생성
2. 맨 위에 아래 형식(front matter) 작성:
   ```
   ---
   layout: post
   title: "글 제목"
   date: 2026-09-08 12:00:00 +0900
   ---
   ```
3. 그 아래에 마크다운으로 본문 작성
4. `git add`, `git commit`, `git push` 하면 몇 분 안에 https://hayoung.work 에 자동 반영됨

## 처음 설정 (한 번만)

1. GitHub 저장소(`j0ah0-work/hayoung.work`)를 Public으로 전환 (또는 Private 유지 시 GitHub Pages는 Private 저장소에서도 동작함)
2. 이 폴더 내용을 저장소에 push
3. 저장소 **Settings → Pages**
   - Source: `Deploy from a branch`
   - Branch: `main` / `(root)`
4. 같은 Pages 설정 화면의 **Custom domain**에 `hayoung.work` 입력 후 저장
5. 도메인 등록업체(가비아/후이즈 등)의 DNS 설정에서 A 레코드 4개 추가 (apex 도메인용):
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
6. DNS 전파 후(수분~수시간) Pages 설정에서 **Enforce HTTPS** 체크
