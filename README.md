# openc906-waves

OpenC906 학습용 유닛 테스트의 시뮬레이션 파형을 브라우저에서 보는 정적 사이트입니다.

- 사이트: https://hyukyeon.github.io/openc906-waves/
- 소스(테스트, 테스트벤치, 학습 노트): https://github.com/hyukyeon/openc906/tree/study/smart_run/study

이 저장소의 내용은 소스 저장소에서 `make site` (`tools/wave_web.py export`)로 생성합니다. 직접 수정하지 마세요.

| 경로 | 내용 |
|---|---|
| `index.html`, `tests.json` | 테스트 목록 |
| `waves/<test>.fst` | 파형 (Verilator 시뮬레이션 VCD 를 FST 로 변환) |
| `cmds/<test>.sucl`, `cmds/<test>/m<n>.sucl` | Surfer 시작 명령: 신호 그룹, MARK 별 확대 |
| `files/<test>/*.txt` | 테스트 소스, objdump, console 로그, pipeview |
| `surfer/` | [Surfer](https://gitlab.com/surfer-project/surfer) 웹 빌드 |

## 라이선스

- 파형과 테스트는 [OpenC906](https://github.com/XUANTIE-RV/openc906) (Apache-2.0) RTL 을 시뮬레이션한 결과입니다.
- `surfer/` 는 Surfer 프로젝트의 빌드 산출물이며 EUPL-1.2 를 따릅니다 (`surfer/LICENSE-EUPL-1.2.txt`, 소스: https://gitlab.com/surfer-project/surfer).
