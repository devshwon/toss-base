# CLAUDE.md

이 저장소(toss-base)는 **Apps in Toss WebView 기반 미니앱**을 **React + TypeScript**로 빠르게 만들기 위한 템플릿입니다.

## 작업 규칙 (필수)

작업 규칙의 단일 원본(Single Source of Truth)은 `.cursor/rules.md`입니다. 모든 작업 전에 아래 규칙을 따르세요.

@.cursor/rules.md

## 빠른 참조

- **스택**: `@apps-in-toss/web-framework` 2.6.1, `@toss/tds-mobile` 2.4.0, `@toss/tds-mobile-ait` 2.4.0
- **개발 서버**: `granite dev` (= `npm run dev`)
- **배포 빌드**: `ait build` (= `npm run build`) — 산출물 경로는 `granite.config.ts`의 `outdir`와 반드시 일치
- **SDK 마이그레이션 점검**: `npx ait migrate`
- **공식 문서**: https://developers-apps-in-toss.toss.im
- **디자인 토큰**: `desigin/toss-look.md`, `src/design/tokens.ts` (임의 px 하드코딩 금지, 토큰만 사용)

## 추가 컨텍스트

- `llms.txt`: LLM용 프로젝트 요약
- `prompts/`: 작업 단계별 표준 프롬프트(charter / packet / review / checklist 등)
- `README.md`: 템플릿 구조 및 최초 치환 포인트
