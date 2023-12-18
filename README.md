## 팀 L.A 캡스톤디자인 1 VR프로젝트 UDon 활용 디지털동화책
---

### 참여자명단

20183320 박지욱 (팀장 / 기획 / 디자인)

20183301 김성호 (기획보조 / 개발)

20183307 김준 (개발)

20183329 양원웅 (디자인)

20183333 유승우 (디자인)

---

### 실행 환경 및 시스템 요구 사항

Unity(2019.4.31f1 LTS)

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/7129d5c3-6bea-448c-93d4-c46c12c185e7)


VR기기 환경 (퀘스트2)

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/fa2d4ac8-1e38-4744-8623-243a367c621a)


VRCHAT

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/b37bf9b1-3457-4e18-99aa-5c64b9c0e93a)

시스템 요구 사양 참고 : [VRCHAT 나무위키](https://namu.wiki/w/VRChat#s-2)

---

### 프로젝트 파일 적용 방법

1. Unity Package File 모든 파일 다운로드, 압축풀기
2. 유니티 패키지 파일 실행
3. VRCHAT 계정 연결

### VRCHAT 회원 가입 및 로그인

프로젝트 내에서 VRCHAT 관련 기능을 이용하기 위해서는 VRCHAT 계정이 필요하다. 
(STEAM 환경 로그인에서는 관리자 및 개발자 기능을 이용하지 못한다.)

VRCHAT 홈페이지 접속 [VRCHAT 홈페이지](https://hello.vrchat.com/)

STEAM 계정이 아닌 자체 계정을 생성하여 활용한다. 

### 프로젝트 파일 내에서 게임 실행 방법

#### 프로젝트 세팅

새 빈 3D 프로젝트 생성

프로젝트 플랫폼 PC 환경 설정 (Window, MAC, Linux) 

#### UDON SDK 불러오기

VRCHAT 로그인 후, 다운로드 페이지에서 SDK 다운로드 [SDK 다운로드 페이지](https://vrchat.com/home/download)

<img width="307" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/0ee59bd3-2f51-46ec-9179-3901b49e3dc3">

다운받은 패키지를 유니티에서 오픈한다.

<img width="165" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/71ac82d6-c1f6-4614-97ac-e8d036a21bfd">

UDON이 적용되어 프로젝트를 활용 가능하다.

#### VRCHAT 월드 빌딩 및 실행

<img width="297" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/a0dccfa5-e433-479f-86fc-85f7f0820bf4">


1.  UDON 패키지와 VRCHAT 게임이 설치된 상태에서 유니티 프로젝트 창 상단의 "VR Chat SDK"를 선택 후, "Show Control Panel"을 선택하여 설정 창을 연다.
2.  "Authentication" 탭에서 VRCHAT 아이디로 로그인(Sign in)
3.  제작한 프로젝트를 실행하기 위해 "Settings" 탭에서 하단의 "Edit"버튼을 눌러 자신의 VRCHAT 실행파일 설치경로를 선택한다.

<img width="397" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/085e27b1-1527-4074-9909-d24e9d80f93b">


4.  "Builder" 탭에서 "Setup Layers for VR Chat" 버튼을 통해 레이어 설정, "Set Collision Matrix" 버튼을 통해 콜리전 행렬 재설정
5.  "Force non-VR"을 체크하고 "Build & Test" 버튼을 눌러 프로젝트 빌딩, VRChat 실행.
6.  만든 맵, 기능을 인게임에서 테스트 진행 가능.  

실행방법 세부 참고 [실행방법 가이드 블로그 글](https://gongdolhoon.tistory.com/entry/UnityVR-Chat-SDK-7-Udon-%EC%98%88%EC%A0%9C-%EB%B9%8C%EB%93%9C%ED%95%B4%EB%B3%B4%EA%B8%B0)

참고 문헌 :

[UDON 시작 가이드](https://creators.vrchat.com/worlds/udon/)

[빌딩&테스트](https://creators.vrchat.com/worlds/udon/getting-started-with-udon/)

[유니티 버전 설정](https://gongdolhoon.tistory.com/entry/UnityVR-Chat-SDK-%EC%9C%A0%EB%8B%88%ED%8B%B0-%EB%B2%84%EC%A0%84-%EC%84%A4%EC%A0%95?category=836424)

[VRCHAT 월드 업로드](https://gongdolhoon.tistory.com/entry/UnityVR-Chat-SDK-World-%EC%97%85%EB%A1%9C%EB%93%9C%ED%95%98%EA%B8%B0?category=836424)

---

#### 메타퀘스트2 및 VR 기기에서 VRCHAT 실행 및 업로드 한 맵 접속
1. 기본 VR기기 초기 설정 완료
[메타퀘스트 초기 설정 가이드](https://www.meta.com/ko-kr/help/quest/articles/getting-started/getting-started-with-quest-2/) 

2. PC에 VR기기를 연결하고, 스팀VR을 실행

[메타퀘스트2 기준 스팀VR 실행방법](https://blog.naver.com/12512512/222893398476)

<img width="673" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/79bef45f-84e5-4e95-8cc8-d8a3c90126de">


3. VRCHAT 라이브러리 게임 설치 후, 실행, 계정 로그인 

<img width="669" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/ed71a0ed-e30f-450d-a4d5-e2048fcc550e">


4. 자신이 업로드한 맵의 이름을 월드 목록 검색창에서 검색 후, 접속

<img width="670" alt="image" src="https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/32a6bda3-af46-471b-99fc-8489cfa1b7cc">

검색이 되지 않는다면 업로드 설정 재확인 바람. 

---


### 로직 설명

1. Animation play trigger
플레이어가 이동중 특정 오브젝트와 충돌을 하였을경우, 에니메이션을 재생하는 로직

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/75949ffc-01ac-466f-9043-d50b7c1ab36e)

2. key box
오브젝트가 충돌을 감지하고 지정된 이름의 오브젝트가 충돌하였을 경우 지정된 애니메이션을 재생함 

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/4df114db-492b-4818-9ba6-a547a992f196)

3. nareition2
플레이어가 이 로직을 가지고 있는 오브젝트와 상호작용을 하면 bool값을 계산하여 false로 되어있던 bool값을 true로 변환하여 애니메이션과 오디오를 재생하여 나레이션을 송출한다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/d7b7d182-96b9-406a-817d-d31e87eceaf8)

4. south Door2
GetBool 이벤트는 South Door2 개체의 isOpen 속성의 값을 가져옵니다. 이 속성은 true이면 문이 열려 있음을 나타내고 false이면 문이 닫혀 있음을 나타냅니다.
SetBool 이벤트는 South Door2 개체의 isOpen 속성의 값을 설정합니다. 이 이벤트는 true 값을 전달하면 문을 열고 false 값을 전달하면 문을 닫습니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/a3d63647-95f9-4dce-9763-ad69ba4d9d70)

5. skybox changer
먼저 Event 노드가 Interact 이벤트를 수신하면 Branch 노드를 사용하여 Interact 이벤트를 발생시킨 개체의 index를 가져옵니다.
index 변수를 사용하여 SkyBoxies 배열의 해당 개체에 액세스합니다.
SkyBoxies 개체의 isOpen 속성의 값을 가져옵니다. 이 속성은 true이면 개체가 열려 있음을 나타내고 false이면 개체가 닫혀 있음을 나타냅니다.
isOpen 속성의 값이 true이면 SetBool 이벤트를 발생하여 SkyBoxies 개체의 isOpen 속성을 false로 설정합니다.
isOpen 속성의 값이 false이면 SetBool 이벤트를 발생하여 SkyBoxies 개체의 isOpen 속성을 true로 설정합니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/f0167f6b-3526-4090-8a2a-4e18cd523082)

5-1. skybox changer
Event 노드는 다른 노드에서 이벤트를 수신하는 데 사용됩니다. 이 경우  Event  노드는  Interact  이벤트를 수신합니다.
Branch  노드는 두 가지 경로 중 하나를 선택하는 데 사용됩니다. 이 경우  Branch  노드는  Interact  이벤트를 발생시킨 개체의  index를 사용하여 두 가지 경로 중 하나를 선택합니다.
GetLength  노드는 배열의 길이를 가져오는 데 사용됩니다. 이 경우  GetLength  노드는  SkyBoxies  배열의 길이를 가져옵니다.
Addition  노드는 두 값을 더하는 데 사용됩니다. 이 경우  Addition  노드는  index  변수와  GetLength  노드의 출력을 더합니다.
Greater ThanOrEqual  노드는 두 값을 비교하여 큰 값이 작은 값과 같거나 크면  true를 반환하는 데 사용됩니다. 이 경우  Greater ThanOrEqual  노드는  index  변수와  GetLength  노드의 출력을 비교하여  index  변수가  GetLength  노드의 출력과 같거나 크면  true를 반환합니다.
즉, 이 로직은 SkyBoxies 배열에 있는 모든 개체의 SkyBox를 newValue 변수의 값으로 변경합니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/b56fbaa9-3f42-44d4-b242-cf754cae1d98)

6. 먼저 Event 노드가 Interact 이벤트를 수신하면 Branch 노드를 사용하여 Interact 이벤트를 발생시킨 개체의 instance를 가져옵니다.
instance 변수를 사용하여 Directional Light 개체를 찾습니다.
Directional Light 개체의 intensity 속성의 값을 가져옵니다. 이 속성은 float 값으로, 밝기를 나타냅니다.
newValue 변수에 새 밝기를 저장합니다.
SetFloat 이벤트를 발생하여 Directional Light 개체의 intensity 속성을 newValue 변수의 값으로 설정합니다.
즉, 이 로직은 Interact 이벤트를 발생시킨 개체가 Directional Light 개체인 경우 newValue 변수의 값으로 Directional Light 개체의 밝기를 변경합니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/5ad28c34-a71b-4ac1-b454-5c744e782c40)

7. tototext
이 로직은 Trigger라는 이름의 개체가 활성화되면 SendCustomEventDelayed 이벤트를 발생시켜 newtaget라는 이름의 개체의 eventName 이벤트를 delaySeconds 초 후에 발생시키는 데 사용됩니다. 로직은 다음과 같이 작동합니다.
먼저 Event 노드가 Trigger 개체의 interact 이벤트를 수신하면 SetFloat 이벤트를 발생하여 delaySeconds 변수의 값을 설정합니다.
delaySeconds 변수의 값이 0보다 크거나 같으면 SendCustomEventDelayed 이벤트를 발생시켜 newtaget 개체의 eventName 이벤트를 delaySeconds 초 후에 발생시킵니다.
즉, 이 로직은 Trigger 개체가 활성화되면 newtaget 개체의 eventName 이벤트를 delaySeconds 초 후에 발생시킵니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/0f72a72d-9487-4266-a159-25c23b68b688)

8. player tp
이 로직은 Trigger라는 이름의 개체가 활성화되면 LocalPlayer 개체의 TeleportTo 이벤트를 발생시켜 teleportPos라는 이름의 Vector3 변수에 저장된 위치로 플레이어를 순간이동시키는 데 사용됩니다. 로직은 다음과 같이 작동합니다.
먼저 Event 노드가 Trigger 개체의 interact 이벤트를 수신하면 SetVector3 이벤트를 발생하여 teleportPos 변수의 값을 설정합니다.
teleportPos 변수의 값이 Vector3.zero이 아니면 LocalPlayer 개체의 TeleportTo 이벤트를 발생시켜 플레이어를 teleportPos 변수의 값으로 순간이동시킵니다.
즉, 이 로직은 Trigger 개체가 활성화되면 LocalPlayer 개체의 TeleportTo 이벤트를 발생시켜 플레이어를 teleportPos 변수의 값으로 순간이동시킵니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/f4f6bc51-3f0e-48c1-938f-eb881c1c922a)

9. 이 로직은 Trigger라는 이름의 개체가 활성화되면 LocalPlayer 개체의 PlaySound 이벤트를 발생시켜 soundName이라는 이름의 string 변수에 저장된 사운드를 재생하는 데 사용됩니다. 로직은 다음과 같이 작동합니다.
먼저 Event 노드가 Trigger 개체의 interact 이벤트를 수신하면 SetFloat 이벤트를 발생하여 volume 변수의 값을 설정합니다.
volume 변수의 값이 0보다 크거나 같으면 LocalPlayer 개체의 PlaySound 이벤트를 발생시켜 soundName 변수의 값을 volume 변수의 값으로 재생합니다.
즉, 이 로직은 Trigger 개체가 활성화되면 LocalPlayer 개체의 PlaySound 이벤트를 발생시켜 soundName 변수의 값을 volume 변수의 값으로 재생합니다.

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/af56bf59-e093-4a62-8680-4ec45594c8b4)


### 참고 문헌 및 자료

VRchat: https://docs.vrchat.com/docs/setting-up-the-sdk

충돌 이벤트: https://www.youtube.com/watch?v=0cOQufJb0f4

teleport: https://www.youtube.com/watch?v=O_8zGfhdzk0

나레이션: https://www.youtube.com/watch?v=cQ3hWKY-NiA

trigger door: https://www.youtube.com/watch?v=8gm7MVAby1w&t=1s

### 프로그램 실행 사진

1. 플레이어가 일정 위치에 다다르면 이벤트 트리거 발동

![3-3](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/4451e068-bcf0-42aa-b8f5-2e0ad581f5c8)

![3-4](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/521b4cfb-b6e3-4843-bfa5-f17ed2793755)

![3-2](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/069198ba-53fa-4da0-955d-2ef1e4b7037b)


2. 올바른 오브젝트를 트리거 설정 위치에 가지고 가면 이벤트 발생

![5](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/ed9b01de-3b6e-4cc1-8ede-51faef23298d)

![5-1](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/836c5a6b-60f5-4947-898e-de72b938b49e)

![5-2](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/5e56503c-122b-41f8-9bd2-e681c55523a9)


3. 플레이어가 일정 위치에 다다르면 이벤트 트리거 발동 (애니메이션 + 사운드)

![5-3](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/03de99c4-1a25-4208-874b-bec9ef310ea5)

![5-4](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/6cf7d9bb-c8c7-4e28-91c8-430195d9bb6d)
