# Number Games public copy

이 폴더의 `copy.json`은 공개 게시용 앱 문구입니다. 게임 소스나 비공개 설정은 이 폴더에 넣지 않습니다.

GitHub의 별도 공개 저장소에 이 폴더의 파일만 올리고 Settings → Pages에서 **Deploy from a branch**, **main / (root)**를 선택합니다. 게시 주소는 `https://<GitHub 사용자명>.github.io/<저장소명>/copy.json`입니다. 실제 주소로 JSON이 열리는지 확인한 뒤 앱의 `localization/publication.json`에 넣고 `node build.cjs`로 Android/iOS 앱을 다시 빌드합니다.

이후 번역을 수정할 때는 앱 원본의 `localization/en.json`을 고치고 `node build.cjs`를 실행한 다음 이 폴더의 변경된 `copy.json`만 같은 저장소에 게시합니다. 첫 주소 설정에는 앱 업데이트가 필요하지만, 같은 주소의 문구 변경은 앱 업데이트 없이 반영됩니다.
