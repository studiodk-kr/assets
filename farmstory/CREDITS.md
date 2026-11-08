# 경북귀농일기 자산 출처

모두 CC0(퍼블릭 도메인) — 출처 표기 의무는 없지만 적어 둔다.

| 파일 | 원본 | 작가 | 라이선스 |
|---|---|---|---|
| `m/nature.glb` | Stylized Nature MegaKit — 덤불 2·꽃 1·풀 3·클로버·풀포기·바위 3·자갈 3·버섯·디딤돌 3 (18종, 그림 512px webp 로 줄임) | Quaternius (https://quaternius.itch.io/stylized-nature-megakit) | CC0 1.0 |

만든 법(2026-10-10): `gltf-transform merge <18개 .gltf> → optimize --texture-compress webp --texture-size 512 --compress false --join false --instance false --flatten false`. 잎·풀 그림은 원래 단색 덩어리(엔진에서 색을 입힘)라 게임이 불러올 때 모양(알파)만 남기고 색을 입힌다(`game/farmstory/p0/js/nature.js`).

## 미니어처 화풍 소품 `m/mini/` (2026-11-08)

Studio DK 가 직접 만든 것. 귀농일기 주소에 `?look=mini` 를 붙였을 때만 쓴다(`game/farmstory/v2/js/mini.js`).

| 파일 | 만든 법 |
|---|---|
| `jangdok.glb` 장독대 · `firewood.glb` 장작 헛간 · `cart.glb` 손수레 · `pyeongsang.glb` 평상 | 원화는 OpenAI 이미지 생성(codex), 3D 는 Stability AI **Stable Fast 3D**(Stability AI Community License — 연 매출 100만 달러 미만 무료, 결과물은 만든 사람 것), 다듬기는 블렌더 5.2(수평 맞추기·바닥 원점·무광). 약 1만 삼각형, 텍스처 1024px |
| `persimmon.glb` 감나무 | 블렌더 코드로 지음(줄기·가지·잎 뭉치·감) — GDI-Apps `game/farmstory/tools/mini/tree.py` |
| `anchae.glb` 안채 · `warehouse.glb` 창고 · `barn.glb` 축사 · `processor.glb` 가공장 · `market.glb` 직판장 · `hall.glb` 마을회관 · `home_a.glb`·`home_b.glb` 마을 집 (2026-11-08) | 소품과 같은 방법(원화 codex → Stable Fast 3D → 블렌더). 블렌더에서 벽을 축에 맞추고 문이 있는 앞면을 남쪽(+z)으로 돌려 구웠다. 약 1만 삼각형, 텍스처 1024px |
| `greenhouse.glb` 비닐하우스 (2026-11-08) | 블렌더 코드로 지음(활대·용마루·밑판·말아 올린 옆 비닐·반투명 비닐·문틀) — GDI-Apps `game/farmstory/tools/mini/greenhouse.py`. 두둑은 게임 코드 |
| `wall.glb` 돌담 1m 조각 · `gate.glb` 기와 대문 · `step.glb` 디딤돌 · `well.glb` 우물 · `clothesline.glb` 빨랫줄 (2026-11-08) | 블렌더 코드로 지음 — GDI-Apps `game/farmstory/tools/mini/yard.py`. 돌담은 게임이 1m 조각을 담 길이만큼 되풀이해 놓는다 |
| `tree_round.glb`·`tree_round2.glb` 둥근 나무 · `tree_kaki.glb` 감나무 · `tree_ginkgo.glb` 은행나무 · `tree_zelkova.glb` 정자나무 · `tree_pine.glb` 소나무 · `bush.glb` 덤불 · `bush_flower.glb` 꽃 덤불 · `flowers.glb` 꽃 무더기 (2026-11-08) | 블렌더 코드로 지음 — GDI-Apps `game/farmstory/tools/mini/trees.py`. 잎 재질(`leafTop`·`leafMid`·`leafLow`)은 게임이 계절 색을 입힌다 |
| `crops.glb` 작물 — 밭 작물 11가지(상추·시금치·부추·미나리·감자·고구마·마늘·참외·딸기·연근·산나물)와 과일나무 4가지(감·자두·포도·사과)를 4단계씩, 물체 60개 (2026-11-08) | 블렌더 코드로 지음 — GDI-Apps `game/farmstory/tools/mini/crops.py` |
