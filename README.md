# 인테리어 계획 (공급 61㎡ / 전용 42㎡)

정적 사이트 — 빌드 없이 Vercel에 그대로 배포됩니다 (Framework Preset: Other).

```
index.html          # 10장 슬라이드 (평면도, 공간별, 콘센트 계획)
images/
  entry/            # 현관
  kitchen/          # 주방
  util/             # 다용도실
  bath/             # 화장실
  small/            # 작은방
  balL/             # 작은방 발코니
  living/           # 거실
  balcony/          # 베란다(거실 발코니)
```

## 레퍼런스 사진 추가
1. `images/<공간>/` 에 사진을 넣고
2. `index.html` 의 `<script id="ref-data">` 목록에 `{"src": "...", "title": "..."}` 를 추가합니다.
   키: entry, kitchen, util, bath, small, balL, living, balcony, balcony-sash

## 콘센트 배치
- 기본 배치는 `index.html` 의 `<script id="outlet-data">` 에 있습니다.
- Vercel 주소에서 편집·저장하면 각자 브라우저에만 저장됩니다. **배치 복사**로 JSON을 복사해 `outlet-data` 에 붙여넣으면 기본값이 됩니다.
