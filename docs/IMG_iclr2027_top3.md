# 이미지 명세서 · ICLR 2027 만점 3편 — 연구실 모의 심사회

> 페이지: `index.html` · 그림체: 캐릭터 팩 18-3 (16비트 RPG풍 픽셀아트, 굵은 어두운 외곽선, 밤의 연구실 남보라 조명) · 그림 안에 글자·숫자·로고를 넣지 않는다.
> 지금 페이지는 그림 없이도 완성 상태(대체 표지 = 캔버스 + 캐릭터 팩 표정 그림). 아래 그림을 받으면 `data-img` 키 자리에 넣는다.

## 1. 필요한 그림 전체

| 키 | 판 | 크기 | 상태 | 쓰는 자리 |
|---|---|---|---|---|
| `cover_iclr27` | 표지 E | 1600×900 (16:9) | **새로 그림** | 맨 위 표지, og:image, 목차 썸네일(잘라 쓰기) |
| `bg_iclr27_hero` | 배경 F | 1600×900 | **새로 그림** | 히어로 뒤 배경(불투명도 0.2~0.35) |
| 캐릭터 표정 39장 | 기본 팩 | 96px | 재사용 | 말풍선·식구 카드·대결 머리 |
| 동작 S11·S12·M14·M15·X1A~X3A | 동작 팩 fight 1.2 | 128 스트립 | 재사용 | 대결 무대(시아 깃발, 모아 응원, 관중석) |

## 2. 새로 그릴 그림

### `cover_iclr27` — 표지 (먼저 받기: 그림체 확인용)

- 장면: 밤의 연구실이 작은 학회 심사장으로 꾸며져 있다. 긴 심사석 책상 위에 빈 점수판 세 개(초록 테두리, **글자 없음**)가 서 있고, 책상 앞에 종이 더미 산이 쌓여 있다(논문 홍수). 
- 배치(왼쪽 → 오른쪽): 인턴 시아(심판 깃발을 든 차분한 자세) · 박사(손을 들어 앞을 가리킴) · 조수 하루(서류를 품에 안고 놀란 눈) · 초파리 연구원(돋보기로 종이 더미를 들여다봄) · 주판봇(주판을 들고 신남) · 인턴 모아(응원하는 주먹). 뒤쪽 어두운 관중석에 미공개 실루엣 셋(흰 점 눈만 보임, 보라 림라이트).
- 키 비율: 박사 1.00 · 조수 0.90 · 시아 0.88 · 모아 0.84 · 주판봇 0.72 · 초파리 0.41.
- 왼쪽 위 40%는 제목 글자를 HTML로 얹을 자리이므로 비워 둔다(어두운 하늘·별빛).

**프롬프트 (영어, 그대로 붙여 넣기)**

```
16-bit RPG pixel art, bold dark outlines, 2-3 step shading, night laboratory turned into a small academic review hall, deep indigo-violet background (#1b1533 to #13141f), purple ceiling light, teal monitor glow, small neon pink and green accents.
A long judging desk at the back right with three blank square score boards with glowing green frames (NO text, NO numbers). A huge pile of paper manuscripts in front of the desk like a small mountain.
Six characters standing in a row in front, left to right:
1) calm girl maid intern, long straight jet-black hair with side-swept bangs, no headdress, gray eyes, small silver drop earrings, charcoal-black long-sleeved maid dress, large gray bow, long white frilled apron, holding a small white referee flag;
2) chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, raising one hand and pointing forward, faint purple sparks in the hand;
3) girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, hugging a stack of papers, surprised eyes;
4) small anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, looking into the paper pile with a magnifying glass;
5) boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and happy mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, holding a wooden abacus;
6) gentle girl maid intern, long ash-beige wavy hair, white frilled maid headband with a ribbon over the left ear, amber-brown eyes, red and navy plaid bow tie, camel knit cardigan, white frilled apron, black skirt, cheering with a raised fist.
Height ratio: scientist 1.00, pink-haired researcher 0.90, black-haired maid 0.88, beige-haired maid 0.84, robot 0.72, fruit fly 0.41.
In the dark audience seats behind: three cute solid dark navy-black silhouettes with thin purple rim light, two round white dot eyes and pink blush pixels each, one with a pink ribbon, one with teal glasses glint, one with a small yellow bell. Not scary.
Keep the top-left 40% of the image as empty dark starry sky for a title overlay.
No text, no letters, no numbers, no logos, no weapons, no real people or brands. 16:9.
```

### `bg_iclr27_hero` — 히어로 배경

- 장면: 사람 없는 밤의 연구실 심사장. 오른쪽 위에 겹눈 벌집 무늬처럼 보이는 육각 조명, 책상 위 빈 점수판 세 개, 바닥에 흩어진 종이. 왼쪽 60%는 어둡고 단순하게(본문 글자가 얹힘).

```
16-bit RPG pixel art background, empty night laboratory review hall, no characters, deep indigo-violet palette (#1b1533 to #13141f), hexagonal honeycomb ceiling lights in the top right, a judging desk with three blank glowing green-framed score boards (no text), scattered manuscript papers on the floor, teal monitor glow, small neon pink and green lab lights. Left 60% dark and simple for text overlay. No text, no numbers, no logos. 16:9.
```

## 3. 일관성 지침

- 캐릭터 고정 외형은 캐릭터 팩 18-4를 바꾸지 않는다. 박사·조수·시아·모아는 좌우 뒤집기 금지.
- 점수판에 "4"를 그려 넣지 않는다(숫자는 페이지가 HTML·캔버스로 그림).
- 생성 도구에 넘길 때 참고 그림: 기본 표정 E13(박사·조수·초파리·주판봇·시아·모아), 미공개 x1~x3 E13, 단체 사진 `images/_sheets/lab6_lineup.png`.

## 4. 넘겨받은 뒤 처리

1. `build_character_pack.py --ingest ./받은그림 --plates cover_iclr27=E,bg_iclr27_hero=F --out received_iclr27`
2. 나온 `Object.assign(SPRITE,{...})` 조각을 페이지 스크립트에 붙이고, `.cover`의 캔버스 대신 표지 그림을 배경으로 쓴다(표지 포함 600 KB 이하).
3. 표지에서 1200×630을 잘라 `og:image`로, 480×270을 목차 썸네일로.

## 5. 체크리스트

- [ ] 그림 안 글자·숫자 0
- [ ] 키 비율·좌우 방향 맞음
- [ ] 미공개 실루엣은 정체를 짐작할 단서 없음
- [ ] 결과(승패)를 암시하는 표정 없음 (표지는 대결 전 장면)
