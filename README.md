# SimonKDesign

> 예술·디자인 작업 오케스트레이션 플러그인

오케스트레이션 진입점: `/skdesign`

## 설치
```
/plugin marketplace add Simon-YHKim/SimonKDesign
/plugin install simonk-design@simonk-design
```

## 의존
SimonKCore 권장 동반 설치 (agent-delegate, model-router, instincts 등 공유 인프라). 없으면 일부 기능 제한.

## 구조
- `skills/` — 도메인 스킬
- `agents/` — 서브에이전트
- `commands/` — 슬래시 커맨드

## 수록 스킬 (20개)

진입점 `/skdesign` 가 의도를 진단해 아래 스킬로 라우팅합니다. 개별 직접 호출도 가능.

`building-native-ui` · `coloring-art` · `consistency-guard` · `design-consultation` · `design-html` · `design-review` · `design-shotgun` · `design-system-keeper` · `design-system-page` · `logo-generator` · `office-docs` · `photo-album` · `plan-design-review` · `remotion-best-practices` · `scientific-paper` · `simon-design-first` · `skdesign` · `slides` · `social-graphic` · `stitch-design-flow`
