# [SFC] 크로노 트리거 한글패치

슈퍼패미콤 **크로노 트리거** 한글패치입니다. 슈퍼패미콤 실기에서 구동하는 것을 목표로 작업했습니다.

- 블로그 소개글: https://dwyn.tistory.com/6
- 최신 버전 다운로드: [Releases](../../releases/latest)
- 버그 제보: [Issues → 버그 제보](../../issues/new/choose)
- 후원: https://litt.ly/dwyn

## 작업 사항 및 변경 이력

주요 작업 사항, 추가 기능, 변경 이력 등 자세한 내용은 **[블로그](https://dwyn.tistory.com/6)** 글을 참조해 주세요.

본 한글패치의 정보를 공유하실 때는 블로그 패치 글로 링크를 걸어 주세요.

## 적용 방법

1. [Releases](../../releases/latest)에서 패치 파일을 받습니다.
2. 직접 가지고 계신 원본 ROM에 패치를 적용합니다.
   - 웹에서 적용: [ROM Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)
   - PC 프로그램: Delta Patcher, Floating IPS 등
3. 패치된 ROM을 에뮬레이터나 플래시카트로 실행합니다.

### 체크섬 확인

패치는 **헤더 없는 일본판 원본 ROM**(4,194,304바이트)에 적용해야 합니다. 패치 후 ROM은 6,291,456바이트로 커집니다.

| 구분 | CRC32 | MD5 | SHA1 |
|---|---|---|---|
| 원본 ROM (일본판) | `4D014C20` | `9D56FB54AF198D43DCD62550767999DF` | `A82F0FBA9BB111FFD0A878853A4563917D9B67BB` |
| 패치 후 (v0.92, 6,291,456바이트) | `4B0CA6F7` | `8D562A2D769C54175403E5AED9C36DA4` | `0184D23D535F899DCF16632A4CE234AC28FB57D9` |

- ROM Patcher JS에 ROM 파일을 넣으면 CRC32, MD5, SHA1이 바로 표시됩니다.
- 크기가 4,194,816바이트인 ROM은 512바이트 헤더가 붙은 파일이니, 헤더를 제거한 뒤 적용해 주세요.

> 이 저장소에는 패치 파일만 있습니다. ROM 파일이나 패치를 적용한 ROM은 배포하지 않으며, 요청에도 응하지 않습니다.
