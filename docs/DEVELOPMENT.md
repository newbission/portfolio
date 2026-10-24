# 사이트 실행·수정 안내

이력서와 프로젝트 사례를 한 곳에서 보여주는 정적 사이트입니다.

저장소 루트 디렉터리를 기준으로 실행합니다.

## 실행

```sh
python3 -m http.server 4173 --directory dist
```

`http://localhost:4173`를 엽니다. 별도 빌드나 패키지 설치가 필요하지 않습니다.

## 수정 위치

- `dist/data.js`: 프로젝트 설명·역할·처리 단계·기술
- `dist/app.js`: 소개·이력서·프로젝트 목록 및 상세 페이지
- `dist/style.css`: 디자인·반응형·PDF 인쇄 스타일
- `dist/index.html`: 기본 구조·메타데이터

이력서의 ‘인쇄 / PDF 저장’ 버튼은 브라우저 인쇄 대화상자를 엽니다. 대상에서 PDF 저장을 선택할 수 있습니다.

## 배포

`main`에 push하면 GitHub Actions가 `dist/`를 GitHub Pages로 배포합니다.

도식은 설명용 재구성입니다. 실제 운영 화면·내부 설정이나 개인 연락처는 포함하지 않습니다.
