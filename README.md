# 프로젝트 좀보이드 한글화 파일 모음(피드백용)

번역 파일 확인 및 피드백 방법

1. 확인하고 싶은 파일의 종류(모드 파일인지 바닐라 파일인지)에 따라 Mods(모드) 혹은 Vanilla(모드X) 폴더로 들어간다 
2. 들어간 폴더 안에서 원하는 모드를 찾아 폴더로 들어간 뒤 파일을 찾거나, 바닐라의 경우 원하는 파일을 찾아 클릭한다.
3. 파일을 그대로 보거나, 원문과 비교하며 보고 싶다면 Raw Blame이 쓰여 있는 텍스트 윗부분 메뉴에서 오른쪽에서 세 번째 아이콘을 클릭하여 내용을 전체 복사한 뒤, 메모장 등의 텍스트 편집기에 붙여넣기하여 본다.
4. 폴더를 전체 다운로드받고 싶을 경우 메인 화면(링크 처음 눌렀을 때 나온 화면으로, 화면 상단 파란색 부분에서 PZ_KO_Translation을 클릭하여 이동 가능)에서 초록색 Copy를 누른 뒤 Download ZIP을 눌러 압축폴더를 받는다.
5. 수정사항이나 번역 명칭 제안 등 피드백이 생기면 [링크가 올라왔던 게시물](https://gall.dcinside.com/mgallery/board/view/?id=pzom&no=70562) 댓글에 달거나, 깃허브를 사용할 줄 안다면 이슈에 올리면 된다.
6. 그 외 질문 등도 5번과 마찬가지

**바닐라 번역 중 현재 올라가 있지 않은, 즉 라디오나 비디오테이프가 아닌 부분의 번역 피드백도 항상 받고 있으니 이 부분도 활발히 피드백해 주면 정말로 감사**

## 작업 목록

### 바닐라

**라디오/TV(RadioData_0_KO, RadioData_1_KO)** : 약 36% 완료. 현재 1677번째 대사(////번호 ORIGINAL ~~ 으로 된 부분에서 번호 부분이 1677)까지 번역 완료. (이후에 번역된 것은 미검수된 것으로, 이전 번역자가 번역한 부분임. 작업되지 않은 부분으로 생각하면 됨)

라디오나 TV 원문의 경우 한글 번역 파일 안에 같이 들어 있긴 하지만, 누가 말한 건지 구분하거나 시간대를 구분하려면 다음 링크에서 원하는 방송사를 선택하면 전체 대사를 볼 수 있음 : https://pzwiki.net/wiki/Category:Transcripts

※현재 라디오/TV 파일의 적용 방식이 달라질 것이라는 얘기가 있어 번역은 잠깐 중단된 상태이나 피드백은 계속 받음

**CD/비디오테이프(Recorded_Media_KO)** : 41.65 버전의 경우 100% 완료, 41.66 버전에 추가된 부분의 경우 아직 번역 안 함. 원문은 폴더에 들어 있는 Recorded_Media 파일(41.66 기준) 참고.

### 모드

만약 모드 번역을 업데이트 전에 미리 적용하고 싶다면, 본 게임에서 같은 이름을 가진 텍스트 파일을 찾아 그 안에 번역된 모드 번역 텍스트를 집어넣으면 됨.

예 : 모드에서 번역된 UI_KO 파일을 본 게임에 적용시키려면, 본 게임의 UI_KO 파일을 찾아가 아래와 같이 편집한다.
```
UI_KO = {
    UI_mainscreen_tutorial = "게임 배우기",
    UI_mainscreen_beginner = "처음 사용자용 게임",
    UI_mainscrren_laststane = "마지막 저항",
    
    .
    . (중략)
    .
    
    UI_optionscreen_Search_Mode_Overlay_Effect_Desaturate = "색 변화만 사용",
    UI_optionscreen_Search_Mode_Overlay_Effect_Both = "뿌연 효과와 색 변화 사용",
    UI_optionscreen_Search_Mode_Overlay_Effect_None = "아무런 효과 사용하지 않음",  [<== 바닐라 게임 UI 파일의 마지막 줄(이미 넣어 둔 모드 텍스트가 있다면 예시와 다를 수 있음)]
    (여기에 엔터를 치고 모드 파일 텍스트를 삽입 (아래 중괄호 '}' 와, 윗줄과 같은 원래 파일의 마지막 줄 사이에 삽입)
    UI_trait_gunspecialist = "총기 전문가",
    UI_trait_gunspecialistdesc = "총기에 대한 고급 지식을 가지고 게임을 시작합니다.<br>+2 조준<br>+2 재장전",
    UI_trait_preparedfood = "대비함: 음식",
    
    .
    . (중략)
    .
    
    UI_MoreTraits_Options_AlbinoAnnounce_ToolTip = "햇빛 알레르기 특성을 가지고 있을 때, 햇빛 때문에 고통받게 되면 알림을 받습니다.",
    UI_MoreTraits_Options_MartialDamage = "무술가 피해 표시",
    UI_MoreTraits_Options_MartialDamage_ToolTip = "무술가 특성을 가지고 있을 때, 플레이어가 가하는 피해를 표시하는 팝업이 생깁니다.",
} <== 이렇게 중괄호 안에 넣어야 함
```
  
**Immersive Medicine(이머시브 메디슨)** : 100% 번역 완료. 모드 제작자에게 파일 제공 완료. 본 모드에 적용.

모드 페이지 : https://steamcommunity.com/sharedfiles/filedetails/?id=2709866494

**More Traits(모어 트레잇)** : 100% 번역 완료. 모드 제작자에게 파일 제공 완료. 본 모드에 적용.

모드 페이지 : https://steamcommunity.com/sharedfiles/filedetails/?id=1299328280
