## 팀 L.A 캡스톤디자인 1 VR프로젝트 UDon 활용 디지털동화책
---

### 참여자명단

20183320 박지욱 (팀장 / 기획 / 디자인)

20183301 김성호 (기획보조 / 개발)

20183307 김준 (개발)

20183329 양원웅 (디자인)

20183333 유승우 (디자인)


### 실행 환경 및 시스템 요구 사항

Unity(2019.4.31f1 LTS)

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/7129d5c3-6bea-448c-93d4-c46c12c185e7)


VR기기 환경 (퀘스트2)

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/fa2d4ac8-1e38-4744-8623-243a367c621a)


VRCHAT

![image](https://github.com/aftersen/Team_L.A_Capstone/assets/138434437/b37bf9b1-3457-4e18-99aa-5c64b9c0e93a)

시스템 요구 사양 참고 : [VRCHAT 나무위키](https://namu.wiki/w/VRChat#s-2)


### 프로젝트 파일 적용 방법

1. Unity Package File 모든 파일 다운로드, 압축풀기
2. 유니티 패키지 파일 실행


### 프로젝트 파일 내에서 게임 실행 방법

1.VR 장비 착용

2.VRCHAT회원가입및 로그인 후 Udon다운

3.VRCHAT실행

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
