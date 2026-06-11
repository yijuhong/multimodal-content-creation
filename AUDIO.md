# SOOMPYO AI 오디오 에셋 및 톤 검수

## 문서 범위

이 문서는 이슈 #18의 범위에 맞춰 숨표 / SOOMPYO 광고의 AI 생성 오디오 에셋과 브랜드 톤 정합성을 기록한다.

- 포함: 최종 광고에 사용할 AI 생성 BGM, 생성 도구, 입력 조건, 출력 요약, 파일명, 사용 구간, 톤 검수
- 제외: 시각 에셋 생성, 립싱크 적용, 최종 MP4 편집, 스토리보드 PDF 내보내기
- 기준 문서: `MISSION.md`, `BRAND.md`, `STORYBOARD.md`, `TOOLS.md`

## 최종 오디오 에셋

| 항목 | 내용 |
| --- | --- |
| 에셋 종류 | BGM |
| 생성 도구 | Suno |
| 사용 목적 | 38초 광고 전체에 깔리는 도시적이고 차분한 인스트루멘털 배경음악 |
| 입력 조건 | Instrumental only 옵션 사용, 보컬과 가사 제외 |
| 파일명 | `assets/audio/soompyo_final_bgm_v01.mp3` |
| 원본 길이 | 약 279.984초 |
| 포맷 | MP3, stereo, 48 kHz |
| 최종 편집 사용 구간 | `0:00-0:38` |
| 출력 결과 요약 | 보컬 없이 낮은 도시적 앰비언스와 부드러운 신스 질감 중심으로 SOOMPYO의 짧은 회복 경험을 받치는 BGM |

## 생성 입력

### Title

```text
SOOMPYO Urban Calm BGM
```

### Style

```text
instrumental ambient electronic, downtempo, minimal, calm city night, warm soft synth pads, subtle low percussion, gentle keys, 70-80 bpm, understated, no vocals
```

### Prompt

```text
Instrumental background music for a 38-second wellness beverage advertisement. Mood is urban calm after work in Seoul, short quiet recovery, understated and warm. Start with a low city-night ambience, gently open into soft ivory warmth, and end cleanly for a product CTA. No vocals, no lyrics, no dramatic build, no medical or functional claims, no upbeat pop jingle.
```

## 씬별 적용 메모

| 씬 | 광고 구간 | BGM 적용 방향 |
| --- | --- | --- |
| Scene 01 | `0:00-0:06` | 낮은 도시적 앰비언스로 퇴근 후 긴장이 남아 있는 상태를 받친다. |
| Scene 02 | `0:06-0:12` | 리듬을 과하게 키우지 않고 정적인 번아웃 분위기를 유지한다. |
| Scene 03 | `0:12-0:19` | SOOMPYO가 등장하는 전환 구간에서 질감만 부드럽게 열리도록 사용한다. |
| Scene 04 | `0:19-0:26` | 한 모금 장면의 딥틸에서 아이보리로 바뀌는 조명 전환을 방해하지 않게 낮게 깐다. |
| Scene 05 | `0:26-0:33` | 긴 휴식이 아니어도 나에게 돌아오는 회복감을 차분하게 이어간다. |
| Scene 06 | `0:33-0:38` | 브랜드명, 제품, CTA가 보이는 마지막 5초를 깨끗하게 마무리한다. |

## 톤 검수

- `BRAND.md`의 톤앤매너인 도시적 차분함과 맞도록 보컬 없는 인스트루멘털 BGM을 사용한다.
- 가사와 내레이션이 없으므로 `BRAND.md`의 짧고 담백한 브랜드 보이스를 침범하지 않는다.
- 입력 조건에 의학적 효능, 기능성 주장, 과장된 광고 문구를 포함하지 않았다.
- 과장된 팝 징글이나 극적인 빌드업을 피하는 조건을 넣어 짧은 회복 경험 중심의 메시지를 유지한다.
- 오디오 소스는 직접 녹음 또는 유료 스톡이 아니라 생성형 AI 결과물로 관리한다.

## 최종 편집 핸드오프

- 최종 광고 편집자는 `assets/audio/soompyo_final_bgm_v01.mp3`의 `0:00-0:38` 구간을 38초 광고 전체 BGM으로 사용한다.
- Scene 06의 마지막 CTA가 흐려지지 않도록 마지막 1초 안에서 자연스럽게 페이드아웃한다.
- 이슈 #18 범위에서는 BGM만 사용하며, SFX나 내레이션은 추가하지 않는다.

## 검증 메모

- `MISSION.md`의 AI 생성 청각 요소 포함 요구를 BGM 1개로 충족한다.
- `MISSION.md`의 직접 촬영, 유료 스톡, 유해 콘텐츠 금지 제약과 충돌하지 않는다.
- `TOOLS.md`의 오디오 생성 주 도구인 Suno와 파일명 규칙의 `bgm` 에셋 분류를 따른다.
- `STORYBOARD.md`의 총 38초 러닝타임에 맞춰 사용 구간을 `0:00-0:38`로 지정했다.
