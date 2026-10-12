# 골짜기 제작 도감

스타듀밸리 × 마인크래프트 감성의 정적 제작법 검색 사이트입니다.

## GitHub Pages 배포
1. GitHub에서 `crafting-valley`라는 **Public** 저장소를 생성합니다.
2. 이 폴더 안의 `index.html`, `style.css`, `app.js`, `recipes.json`, `.nojekyll` 파일을 저장소 최상위에 업로드합니다. (ZIP 파일 자체를 업로드하지 마세요.)
3. 저장소 **Settings → Pages → Build and deployment → Source: Deploy from a branch**를 선택합니다.
4. Branch를 `main`, 폴더를 `/(root)`로 선택하고 **Save**합니다.
5. 게시 후 `https://사용자이름.github.io/crafting-valley/`에서 접속할 수 있습니다.

## 데이터 수정
`recipes.json`에서 아이템을 추가/수정합니다. 형식: `{"name":"아이템 이름","materials":[{"name":"재료 이름","qty":2}],"station":"일반 기술대"}`. JSON 형식을 지켜주세요.

## 참고
- 원본: `일반기술대(1).xlsx` / 제작 아이템 65개, 재료 항목 290개
- 엑셀에 기재된 이름과 수량을 최대한 그대로 반영했습니다. `8개` 표기는 숫자 8로 정규화했습니다.
- 공백 차이(예: `화로 기판` / `화로기판`)는 검색 및 하위 제작 연결 시 자동 인식합니다.
- 원본에 `분사노출`, `기계부품4` 등의 이름이 있습니다. 오타일 수 있으므로 게임 내 표기와 대조 후 수정해 주세요.
- 서버에서 직접 제공한 아이템 이미지가 없으므로 현재는 카테고리별 그림문자 아이콘을 사용합니다. 실제 아이콘 PNG를 확보하면 교체할 수 있습니다.
- 즐겨찾기는 브라우저에만 저장됩니다. 다른 기기와 자동 동기화되지 않습니다.
- `index.html`을 파일로 직접 여는 경우 JSON을 읽지 못할 수 있습니다. 로컬 확인은 `python -m http.server 8000` 후 `http://localhost:8000/`에 접속하세요.
