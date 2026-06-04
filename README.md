# Toss InApp 샘플 템플릿

토스 WebView 미니앱을 빠르게 복제해서 쓸 수 있는 최소 템플릿입니다.
SDK 2.x 기준(`@apps-in-toss/web-framework` 2.6.1, `@toss/tds-mobile` 2.4.0, `ait build`)으로 맞춰져 있습니다.

> 빌드 도구: 개발 서버는 `granite dev`, 배포 아티팩트(`.ait`) 빌드는 `ait build`로 수행합니다.
> SDK 업그레이드 시 `npx ait migrate`로 공식 마이그레이션 적용 여부를 확인할 수 있습니다.

## 1) 가장 먼저 바꿀 값

- `granite.config.ts`
  - `appName`
  - `brand.displayName`
  - `brand.icon`
- `index.html`의 `<title>`
- `src/pages/Home.tsx`의 서비스 문구

## 2) 실행

```bash
npm install
npm run dev
```

## 3) 빌드

```bash
npm run build
```

내부적으로 `ait build`가 실행됩니다.

## 4) 템플릿 구조

- `src/App.tsx`: 라우팅 및 토스 backEvent 처리
- `src/pages/Home.tsx`: 홈(메뉴 허브)
- `src/pages/Feature.tsx`: 기능 화면 예시(입력/저장/진동)
- `src/pages/Settings.tsx`: 설정 화면 예시(로컬 저장)
- `src/services/templateStorage.ts`: 설정 저장소

## 5) AI 치환 포인트

- `TODO:` 주석이 있는 위치를 우선 치환
- `Template*` 타입/함수명을 도메인명으로 변경
- `feature`, `settings` 라우트를 실제 서비스 라우트로 변경
