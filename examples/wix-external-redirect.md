# Example — Wix 주소를 유지하면서 외부 사이트로 즉시 이동

## 사용자 목표
기존 Wix 주소와 이미 인쇄된 QR은 그대로 두고, 방문자는 새 외부 홈페이지로 바로 이동하게 한다.

## 잘못된 첫 접근
“Wix 편집기를 PC에서 열어 직접 수정해야 한다.”

문제는 **목표를 Wix 편집기라는 특정 도구에 묶은 것**입니다.

## 더 좋은 탐색
- Wix의 Custom Embed 기능 확인
- HEAD 위치에 ESSENTIAL 스크립트 삽입 가능 여부 확인
- 외부 URL로 `location.replace()` 가능 여부 확인
- 기존 Wix 주소와 QR을 그대로 유지할 수 있는지 확인

## 일반 패턴
```html
<script>
(function () {
  const target = "https://example.com/";
  if (location.pathname === "/your-wix-path") {
    location.replace(target);
  }
})();
</script>
```

## 주의
- 사이트/경로 조건을 정확히 제한할 것
- 실제 공개 URL에서 최종 목적지까지 브라우저로 검증할 것
- 리다이렉트 루프가 없는지 확인할 것
- 사용 중인 플랫폼 정책과 현재 API/Embed 기능을 그때그때 확인할 것

## 재사용 포인트
핵심은 Wix 자체가 아니라 이 사고방식입니다.

**기존 URL/QR 보존 + 새 목적지 이동**이라는 목표라면,
편집기 수동작업 전에 Redirect / Routing / Custom Embed / Proxy / Deployment 설정을 먼저 검토합니다.
