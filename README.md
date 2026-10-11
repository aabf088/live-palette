# LIVE PALETTE

캡처한 이미지의 주요 색상과 포인트 색상 5개를 자동으로 모으는 작은 Mac 메뉴 막대 / Windows 트레이 앱입니다.

## 다운로드

[Windows 11 x64 다운로드](https://github.com/aabf088/live-palette/releases/download/v0.2.0/LIVE-PALETTE-Windows-x64.zip) · [Apple Silicon Mac 다운로드](https://github.com/aabf088/live-palette/releases/download/v0.2.0/LIVE-PALETTE-macOS-arm64.zip) · [릴리스 보기](https://github.com/aabf088/live-palette/releases)

Windows 버전은 0.2.0 베타, Mac 버전은 0.1.3입니다. Intel Mac과 Windows ARM용 배포본은 현재 제공하지 않습니다.

## Windows

1. Windows 11 x64 PC에서 ZIP을 풀고 `LivePalette.exe`를 실행합니다. .NET을 따로 설치하거나 관리자 권한으로 실행할 필요가 없습니다.
2. 작업 표시줄의 숨겨진 아이콘 영역에 있는 팔레트 아이콘을 꺼내 두세요. 아이콘을 클릭하면 감지를 켜거나 끕니다.
3. 감지가 켜져 있을 때 **Win + Shift + S**로 영역을 캡처하세요. 캡처 도구가 클립보드에 보낸 이미지에서 색상 5개가 자동 저장·복사됩니다.
4. **Win + Print Screen**으로 Windows 기본 스크린샷 폴더에 새로 저장한 캡처도 처리합니다.

파일 감지는 Windows의 알려진 Screenshots 폴더(OneDrive로 이동된 경로 포함)를 사용합니다. 별도로 지정한 다른 저장 폴더와 타사 캡처 도구는 첫 버전 범위에 포함하지 않습니다. 일반 앱에서 복사한 이미지는 처리하지 않습니다.

트레이 우클릭 메뉴의 **종료**로 앱을 닫을 수 있습니다. Microsoft 서명 인증서를 적용하지 않은 베타라 SmartScreen에서 알 수 없는 앱으로 표시될 수 있습니다.

## macOS

1. macOS 14 이상 Apple Silicon Mac에서 ZIP을 풀고 `LIVE PALETTE.app`을 응용 프로그램 폴더로 옮겨 실행합니다.
2. 메뉴 막대의 팔레트 아이콘으로 감지를 켜거나 끕니다.
3. 평소처럼 **⌘⇧3** 또는 **⌘⇧4**로 화면을 캡처합니다. 주요 색상 5개가 자동 저장·복사됩니다.

Apple Developer ID 서명과 공증은 아직 적용하지 않았습니다. macOS 보안 설정에 따라 실행이 차단될 수 있습니다. [Apple의 앱 보안 안내](https://support.apple.com/ko-kr/102445)를 확인하세요.

새 스크린샷 파일과 macOS 미리보기를 감지합니다. 보호된 폴더 접근에는 macOS의 허용이 필요할 수 있습니다. Control 키를 함께 눌러 클립보드에만 보내는 캡처는 지원을 보장하지 않습니다.

## 팔레트 사용

- 캡처 후 HEX 코드 5줄이 클립보드에 복사됩니다. 서식을 지원하는 앱에는 색상 네모도 붙여넣습니다. 다섯 줄 전체를 담은 PNG도 제공하므로, 받는 앱에 따라 텍스트·서식 또는 한 장의 이미지로 들어갈 수 있습니다.
- 색상 하나를 클릭하면 해당 색상만 한 줄로 복사합니다.
- 화살표를 펼치면 **현재 팔레트를 제외한 최근 기록 두 개**가 보입니다. 기록을 누르면 다시 불러오고 복사합니다.
- 패널 우클릭 메뉴는 **복사 · 팔레트 저장 · 저장한 팔레트**입니다.
- 앱의 캡처 버튼은 없습니다. 운영체제 기본 단축키로 캡처하세요. 앱이 화면 기록 권한을 요청하거나 직접 촬영하지 않습니다.
- 감지가 켜져 있으면 캡처 후 클립보드가 색상 값으로 바뀝니다.

## 색상 선별

픽셀 면적과 색상 차이로 주요 색상 3개를 고르고, 색상 차이·채도·면적을 함께 고려해 포인트 색상 2개를 채웁니다. 밝은 색부터 어두운 색 순으로 표시합니다. 아주 작은 영역은 잡음으로 제외될 수 있고, 원본의 색이 부족하면 같은 색을 반복합니다.

## 개인정보

분석·저장은 기기 안에서만 처리합니다. 화면 이미지를 외부로 보내거나 앱이 별도로 보관하지 않습니다. 팔레트에는 색상·비율·날짜·원본 파일 이름을 저장합니다.

Windows 기록 위치는 `%LOCALAPPDATA%\LivePalette\palettes.json`, Mac 기록 위치는 `~/Library/Application Support/LivePalette/palettes.json`입니다. 스크린샷 저장이나 클립보드 처리 상황에 따라 감지가 몇 초 늦을 수 있습니다.

## 문의

문제나 제안은 [Issues](https://github.com/aabf088/live-palette/issues)에 남겨 주세요. 재현 방법과 운영체제 버전만 적어도 도움이 됩니다. 개인 정보가 포함된 스크린샷은 첨부하지 않아도 됩니다.

이 저장소는 앱 배포와 사용 안내를 위한 저장소입니다.
