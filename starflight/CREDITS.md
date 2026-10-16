# Starflight: Frontier Hunter 제작 기록

게임 설계·코드·절차형 로봇 외장·리깅·행성 셰이더: Studio DK 프로젝트 제작물.

## 3D 전투기·전함

Quaternius, Ultimate Spaceships Pack, CC0-1.0.

- 원본: https://quaternius.com/packs/ultimatespaceships.html
- 배포 페이지: https://opengameart.org/content/lowpoly-spaceships-pack
- 사용 모델: Spitfire, Insurgent, Imperial. OBJ·원본 텍스처를 GLB로 변환.
- 파일별 SHA-256과 크기: `https://raw.githubusercontent.com/studiodk-kr/assets/main/starflight/manifest.json`.
- 로봇은 외부 다운로드 모델이 아니라 이 게임의 실제 SkinnedMesh·Bone 리그로 제작했다.

## 음악

설치된 ACE-Step 1.5 Turbo로 이 게임을 위해 생성한 연주곡. 외부 상용 곡을 사용하거나 특정 음악가를 모방하도록 요청하지 않았다.

| 장면 | 곡명 | 길이 | 빠르기 | 재생 |
|---|---|---:|---:|---|
| 격납고·상점 | 변경의 격납고 | 1:58 | 82 BPM | 반복 |
| 일반 의뢰 | 열린 항로 | 2:28 | 132 BPM | 반복 |
| 보스전 | 레드라인 | 2:28 | 154 BPM | 반복 |
| 엔딩 | 별들 사이의 귀환 | 1:40 | 92 BPM | 1회 |

총 8분 34초. 앞의 세 곡은 2초 순환 크로스페이드, 모든 곡은 -18 LUFS 목표·-1.5 dBTP 제한으로 후처리했다. MP3 디코딩 검사 통과, 실제 샘플 피크 -2.1~-1.8 dB. 생성 프롬프트·seed·모델·원본/배포 SHA는 `https://raw.githubusercontent.com/studiodk-kr/assets/main/starflight/music/manifest.json`에 기록했다. 청취 취향과 장기 반복 피로도는 사용자 검토 대상이다.

## 라이브러리

Three.js r160 — MIT, 저장소의 `game/shared/vendor/three/`를 사용한다. Pretendard — SIL Open Font License, 저장소 공용 글꼴을 사용한다. 효과음은 Web Audio 합성음이다.

Studio DK 자체 제작·생성 자원의 프로젝트 배포 표기는 저장소 루트 정책(CC BY-NC-ND 4.0)을 따른다. 외부 Quaternius 모델은 원래의 CC0-1.0을 따른다.
