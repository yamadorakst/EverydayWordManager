# 일상단어 매니저 (Black Edition)

안드로이드용 Kotlin 프로젝트입니다.

## 포함 기능
- 검은색 배경과 네온 포인트 UI
- 한국어 일상 단어 목록 내장
- 3/5/10/15/30초 단어 자동 전환
- 시작, 일시정지, 그만, 다음 단어
- 현재 단어 클립보드 복사
- 현재 진행 위치 표시

## 중요 제한
이 앱은 카카오톡에 자동으로 메시지를 보내지 않습니다. 단어를 표시하고 복사하는 보조 도구이며, 테스트 채팅방에 붙여넣고 전송하는 동작은 사용자가 직접 수행합니다.

## APK 빌드
### Android Studio에서
1. Android Studio 최신 버전과 JDK 17을 설치합니다.
2. `File > Open`에서 이 폴더를 엽니다.
3. Gradle Sync가 끝날 때까지 기다립니다.
4. `Build > Build Bundle(s) / APK(s) > Build APK(s)`를 선택합니다.
5. APK는 `app/build/outputs/apk/debug/app-debug.apk`에 생성됩니다.

### GitHub Actions로 클라우드 빌드
프로젝트를 GitHub 저장소에 올리면 `.github/workflows/build-apk.yml`이 APK를 빌드합니다.
1. GitHub에서 새 저장소를 만듭니다.
2. 이 ZIP을 풀고 안의 파일들을 저장소에 업로드합니다.
3. 저장소의 `Actions` 탭에서 `Build Android APK`를 실행합니다.
4. 작업이 성공하면 결과 페이지 아래 `Artifacts`에서 `everyday-word-manager-debug-apk`를 다운로드합니다.

요구 환경: Android Studio, JDK 17, Android SDK Platform 35, Gradle 8.9.
