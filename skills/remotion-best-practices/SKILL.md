---
name: remotion-best-practices
description: >
  Use when the user wants remotion best practices — triggers "Remotion 비디오", "프로그래밍 비디오", "remotion video", "programmatic video", "code-driven video", or /remotion-best-practices. Produces Remotion 으로 프로그래밍 가능한 비디오 (TypeScript + React) — composition, sequences, audio sync, lambda render, 데이터 기반 비디오 생성. 차용 출처 slide deck remotion-best-practices Niche — only for video generation projects. Different from /design-shotgun (visual design exploration) and /make-pdf (document export). This produces actual MP4/WebM rendered video.
version: 1.0.0
allowed-tools:
  - Bash
  - Read
  - Edit
  - Write
---

# /remotion-best-practices

Remotion 으로 프로그래밍 가능한 비디오 (TypeScript + React) — composition, sequences, audio sync, lambda render, 데이터 기반 비디오 생성. 차용 출처 slide deck remotion-best-practices

## When to use

Trigger phrases:
- Korean: Remotion 비디오, 프로그래밍 비디오
- English: remotion video, programmatic video, code-driven video
- Slash: `/remotion-best-practices`

## What it does

Remotion 으로 프로그래밍 가능한 비디오 (TypeScript + React) — composition, sequences, audio sync, lambda render, 데이터 기반 비디오 생성. 차용 출처 slide deck remotion-best-practices

## Boundaries

Niche — only for video generation projects. Different from /design-shotgun (visual design exploration) and /make-pdf (document export). This produces actual MP4/WebM rendered video.

## Operational notes

- 검증 가능 산출물: 사용자가 직접 확인 가능한 파일/URL 우선 생성
- 외부 의존: SKILL body 에 명시 (Vercel CLI, Expo CLI, LaTeX 등)
- 실패 시: 어떤 단계에서 막혔는지 명시, 사용자 결정 받기

## 완료 보고 (HTML) — 표준
작업을 끝내면 **HTML 완료 보고서**를 생성한다 (SimonKCore `completion-report` 표준).
- 첫 화면은 **심플 요약**(한눈 카드 한 줄) + 직관 그래픽/차트(인라인 SVG)·이미지.
- 각 항목 옆 **[자세히] 버튼**(`<details>`)을 펼치면 상세 — 처음부터 쏟지 않는다(progressive disclosure).
- 자체완결 1파일(인라인 CSS/SVG, 무JS) · 사용자 언어 · 현지시간 스탬프.
- Core 있으면 `completion-report` 호출, 없으면 동일 형식으로 인라인 생성.
