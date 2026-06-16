---
name: slides
description: >
  Use when the user wants slides — triggers "슬라이드 만들어", "발표자료 만들어", "피치덱 만들어", "프레젠테이션", "pitch deck", "slide deck", "presentation slides", "html slides", or /slides. Produces zero-dependency HTML 슬라이드 (16:9 고정, embedded CSS/JS). 사용자가 발표 내용 알려주면 LLM 이 3 visual style preview 생성 후 사용자가 하나 선택하면 그 톤으로 전체 deck 생성. PPT 파일도 web 변환 지원. /simon-design-first show-don-t-tell 패턴 적용. 차용 출처 zarazhangrui/frontend-slides Different from /design-html (general HTML) and /design-shotgun (design variants exploration). This is specifically presentation decks with 3-preview pattern.
version: 1.0.0
allowed-tools:
  - Bash
  - Read
  - Write
  - Edit
  - AskUserQuestion
  - SendUserFile
---

# /slides

zero-dependency HTML 슬라이드 (16:9 고정, embedded CSS/JS). 사용자가 발표 내용 알려주면 LLM 이 3 visual style preview 생성 후 사용자가 하나 선택하면 그 톤으로 전체 deck 생성. PPT 파일도 web 변환 지원. /simon-design-first show-don-t-tell 패턴 적용. 차용 출처 zarazhangrui/frontend-slides

## When to use

Trigger phrases:
- Korean: 슬라이드 만들어, 발표자료 만들어, 피치덱 만들어, 프레젠테이션
- English: pitch deck, slide deck, presentation slides, html slides
- Slash: `/slides`

## What it does

zero-dependency HTML 슬라이드 (16:9 고정, embedded CSS/JS). 사용자가 발표 내용 알려주면 LLM 이 3 visual style preview 생성 후 사용자가 하나 선택하면 그 톤으로 전체 deck 생성. PPT 파일도 web 변환 지원. /simon-design-first show-don-t-tell 패턴 적용. 차용 출처 zarazhangrui/frontend-slides

## Boundaries

Different from /design-html (general HTML) and /design-shotgun (design variants exploration). This is specifically presentation decks with 3-preview pattern.

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
