<div align="center">
  
### YoungJungTeam

![프로젝트 기간](https://img.shields.io/badge/프로젝트_기간-2023.11.08~2023.11.29-fab2ac?style=flat)

</div> 

<br>

## 📝 소개
### **VR/AR/게임 제작 기초 기말 프로젝트**

이 프로젝트는 **마법소녀의 마을**을 침략한 **골렘들과 그들의 왕**을 마법을 통해 물리쳐 마을을 지키는 **3D 액션 어드벤처 게임**입니다. 

<br>

## 💡 프로젝트 기획
* **게임 개요**  
  플레이어는 마법소녀 캐릭터를 조작하여 다양한 스킬을 사용해 몬스터와 보스 몬스터를 처치하며 마을을 지킵니다. 기존의 2D 게임 방식이 아닌 3D로 구현하여 Unity의 다양한 기능을 적극 활용하고, 현실감을 높이며 몰입감 있는 게임 경험을 제공하는 것을 목표로 했습니다.
* **주요 목표**  
  - 3D 액션 어드벤처 게임 구현  
  - Unity의 다양한 기능을 활용하여 몰입감 있는 경험 제공  
  - 마법소녀 캐릭터와 몬스터의 상호작용 및 타격감 강조  

<br>

## 🎬 게임 플레이 영상

[![게임 영상 썸네일](https://img.youtube.com/vi/LYk9SU07zkw/0.jpg)](https://youtu.be/LYk9SU07zkw)  
*(위의 이미지를 클릭하시면 유튜브 플레이 영상으로 이동합니다!)*

<br>

## 🖥️ 화면 구성 (Features)

### 1️⃣ 시작 씬 (Start Scene)
게임 조작법과 목표를 알려주는 대기 화면입니다.

| 게임 시작 화면 | 주요 구현 내용 |
| :---: | :--- |
| <img width="500" alt="Start Scene" src="https://github.com/user-attachments/assets/11ccefb4-d8cf-47ff-9eb4-7c0742589228" /> | <ul><li>UI 아이콘을 배치하여 게임 조작법과 해당 키의 기능을 설명합니다.</li><li>UI Button의 `OnClick()` 이벤트를 활용하여, 플레이어가 조작법을 숙지한 후 **Start 버튼**을 누르면 게임 씬으로 이동하도록 구현했습니다.</li></ul> |

### 2️⃣ 게임 씬 (Game Scene)
게임을 직접 플레이하며 전투가 벌어지는 메인 화면입니다.

| 메인 전투 화면 | 주요 구현 내용 |
| :---: | :--- |
| <img width="500" alt="Game Scene" src="https://github.com/user-attachments/assets/77e0ed29-8622-4bb2-a2da-f622ca721fd2" /> | <ul><li>`Input.GetKeyDown`을 사용하여 특정 키 입력 시 다양한 스킬이 발사되도록 액션 로직을 구현했습니다.</li><li>몬스터의 스폰 위치를 지정하고, 일정 시간이 지나면 지속적으로 스폰되도록 구현했습니다.</li><li>Unity의 **NavMesh** 기능을 활용하여 스폰된 몬스터가 플레이어를 추적하도록 AI를 구현했습니다.</li><li>일정 개수의 몬스터를 처치하면 **보스 몬스터**가 등장합니다.</li><li>몬스터와 보스의 공격 패턴을 **근거리/원거리**로 나누어 난이도를 조절했습니다.</li><li>**파티클 시스템(Particle System)**을 이용해 공격 및 피격 이펙트를 추가하여 타격감을 향상시켰습니다.</li></ul> |

### 3️⃣ 게임 종료 씬 (Game Over & Victory Scene)
게임의 결과(승리 또는 패배)를 보여주는 씬입니다.

| 게임 오버 화면 | 게임 클리어(승리) 화면 |
| :---: | :---: |
| <img width="400" alt="Game Over Scene" src="https://github.com/user-attachments/assets/f423c877-a37f-4695-aba8-6110eca16f53" /> | <img width="400" alt="Victory Scene" src="https://github.com/user-attachments/assets/10f87d76-46d8-40b9-bd58-193bea84cdae" /> |

* **결과 화면(Scene) 구성**
  * 플레이어의 체력이나 보스 처치 여부에 따라 승리/패배 씬으로 나뉘어 이동합니다.
  * 결과에 맞는 캐릭터 애니메이션(좌절 또는 환호)을 적용하여 몰입감을 높였습니다.
* **UI 버튼 기능 추가**
  * `OnClick()`을 활용하여 '다시 시작(Restart)' 또는 '게임 종료(Exit)' 기능을 구현했습니다.

<br>

## ⚙ 기술 스택 (Tech Stack)

### Front-end
<img src="https://img.shields.io/badge/Unity-100000?style=for-the-badge&logo=unity&logoColor=white"/> <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white"/>

### Tools
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>

<br>

## 🤔 자체 평가 (Review)

### ✨ 잘한 점
* 기획한 스킬 이펙트에 맞춰 **파티클(Particle)**을 적극적으로 활용함으로써 전투 액션의 퀄리티를 크게 향상시킬 수 있었습니다.
* 맵 제작 시 다양한 소스의 에셋을 조합하여 기획했던 배경 분위기와 가장 유사한 환경을 성공적으로 구축했습니다.
* 강의에서 다루지 않았던 **네비메쉬(NavMesh)** 기능을 스스로 학습하고 적용하여, 몬스터가 플레이어를 자연스럽게 추적하며 이동하도록 구현해냈습니다.
* 공동 작업을 위해 GitHub을 적극 사용하면서 버전 관리 및 협업에 대한 숙련도와 이해도를 크게 높였습니다.

### 💦 아쉬운 점 및 개선 목표
* UI 제작 시 `Scale With Screen Size` 설정과 `Anchor Presets`을 완벽하게 활용하지 못해, 해상도가 다른 기기에서는 UI가 엇나가는 반응형 UI 레이아웃 이슈가 발생했습니다.
* 골렘이 투사체(돌)를 던질 때, 플레이어와의 직선상에 다른 골렘이 있으면 투사체가 통과하지 못하고 앞의 몬스터에 맞는 문제가 있었습니다. (콜라이더 레이어 분리 등 물리 엔진에 대한 추가 학습 필요)
* 몬스터가 사망 처리가 되었음에도 오브젝트가 파괴되기 전에 플레이어와 닿으면 충돌 판정이 남아있어 데미지를 입는 버그를 완벽히 수정하지 못했습니다.
* 근접 공격을 태그 충돌 방식으로 구현했으나, 애니메이션 진행에 따른 관절(팔, 다리)의 세밀한 Transform 위치 변화를 완벽히 트래킹하지 못해, 정확히 주먹이 닿는 타이밍에만 데미지가 들어가도록 하는 정교한 히트박스 구현에는 한계가 있었습니다.

<br>

## 💁‍♂️ 프로젝트 팀원

| 최정환 (Front-End) | 김영준 (Front-End) |
| :---: | :---: |
| <img src="https://github.com/cjh5779.png?size=120" width="120" /> | <img src="https://github.com/youngjoon0405.png?size=120" width="120" /> |
| [@cjh5779](https://github.com/cjh5779) | [@youngjoon0405](https://github.com/youngjoon0405) |
