<div align="center">
  
### YoungJungTeam

[<img src="https://img.shields.io/badge/프로젝트 기간-2023.11.08~2023.11.29-fab2ac?style=flat&logo=&logoColor=white" />]()
</div> 

## 📝 소개
- *VR/AR/게임제작기초 기말 프로젝트*
</br></br>
-프로젝트 기획

  - 마법소녀의 마을을 침임한 골렘들과 그들의 왕을  마법을 통해 물리쳐 마을을 지키는 액션 어드벤처 게임
  - 플레이어가 움직이는 캐릭터를 조작하며 다양한 스킬을 활용해 몬스터를 처치하는 3D 게임을 개발하고자 했습니다. 기존에 수업에서 주로 다뤘던 2D 방식이 아닌 3D로 구현하여, Unity의 다양한 기능을 적극 활용함으로써 현실감을 높이고, 보다 몰입감 있는 게임 경험을 제공하는 것을 목표로 삼았습니다.

<br />

## 화면 구성

### 시작 씬
게임 조작법과 목표를 알려주는 씬입니다.

<div style="display: flex; align-items: center;">
  <img width="400" alt="Start Scene" src="https://github.com/user-attachments/assets/11ccefb4-d8cf-47ff-9eb4-7c0742589228" style="margin-right: 20px;"/>
  <ul>
    <li>UI 아이콘을 배치하여 게임 조작법과 해당 키의 기능을 설명한다.</li>
    <li>UI Button의 <code>OnClick()</code>을 활용하여, 플레이어가 조작법을 숙지한 후 <strong>Start 버튼</strong>을 통해 게임 씬으로 이동할 수 있도록 구현한다.</li>
</ul>
</div>

---

### 게임 씬
게임을 플레이할 수 있는 메인 씬입니다.

<div style="display: flex; align-items: center;">
  <img width="400" alt="Game Scene" src="https://github.com/user-attachments/assets/77e0ed29-8622-4bb2-a2da-f622ca721fd2" style="margin-right: 20px;"/>
  <ul>
    <li><code>Input.GetKeyDown</code>을 사용하여 특정 키를 누르면 다양한 스킬이 발사되도록 구현한다.</li>
    <li>몬스터의 스폰 위치를 지정하고, 일정 시간이 지나면 몬스터가 스폰되도록 구현한다.</li>
    <li>Unity의 <strong>NavMesh</strong> 기능을 활용하여 스폰된 몬스터가 플레이어를 따라오도록 구현한다.</li>
    <li>설정된 개수의 몬스터를 처치하면 <strong>보스 몬스터</strong>가 스폰되도록 구현한다.</li>
    <li>몬스터와 보스의 공격을 <strong>근거리 공격</strong>과 <strong>원거리 공격</strong>으로 나누어 게임의 난이도를 높인다.</li>
    <li><strong>파티클 시스템</strong>을 이용하여 플레이어와 몬스터의 공격에 <strong>이펙트</strong>를 추가해 게임의 퀄리티를 향상시킨다.</li>
  </ul>
</div>

---

### 게임 종료 씬  
게임의 결과를 보여주는 씬입니다.

<div style="display: flex; align-items: center;">
  <img width="400" alt="Game Over Scene" src="https://github.com/user-attachments/assets/f423c877-a37f-4695-aba8-6110eca16f53" style="margin-right: 20px;"/>
  <img width="400" alt="Victory Scene" src="https://github.com/user-attachments/assets/10f87d76-46d8-40b9-bd58-193bea84cdae" />
</div>

<ul>
  <li><strong>결과 화면(Scene) 구성</strong>
    <ul>
      <li>게임 결과(승리/패배 등)에 따라 적절한 씬을 구현한다.</li>
      <li>결과에 맞는 캐릭터 애니메이션을 적용하여 몰입감을 높인다.</li>
    </ul>
  </li>
  <li><strong>UI 버튼 기능 추가</strong>
    <ul>
      <li><code>OnClick()</code>을 활용하여 게임 종료 또는 재시작 기능을 구현한다.</li>
    </ul>
  </li>
</ul>



<br />

## ⚙ 기술 스택
### Front-end
<div>
<img width="90" alt="Image" src="https://github.com/user-attachments/assets/5ea17a38-71d9-4301-b701-e6b51f871b86" />
<img width="90" alt="Image" src="https://github.com/user-attachments/assets/8039f347-29d9-4018-ba79-901e5410484a" />
</div>

### Tools
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Github.png?raw=true" width="80">
</div>

<br />

## 🤔 자체 평가
- **잘한 점**
  - 기획한 스킬 이펙트에 맞춰 파티클 UI를 활용함으로써 스킬의 퀄리티를 향상시킬 수 있었다.
  - 맵 제작 시 다양한 소스에서 에셋을 가져와 기획했던 배경과 유사한 환경을 구현할 수 있었다.
  - 강의에서 다루지 않았던 네비메쉬 기능을 활용하여 몬스터가 플레이어를 추적하며 이동하도록 구현하였다.
  - 공동 작업을 위해 GitHub을 사용하면서 GitHub에 대한 숙련도와 이해도를 높일 수 있었다.

- **아쉬운 점**
    - UI를 제작할 때 Scale With Screen Size 설정과 Anchor Presets을 활용하여 UI를 재배치해야 했지만, 이를 적용하지 않아 해상도가 다른 기기에서는 UI가 원하는 위치에 배치되지 않는 문제가 발생했다.
    - 골렘이 돌을 던질 때, 직선상에 다른 골렘이 배치되어 있으면 플레이어에게 도달하지 않고 앞에 있는 골렘에 맞아 떨어지는 문제와, 골렘이 사망했을 때 스킬 쿨타임이 맞아떨어져 몬스터 오브젝트가 사라지기 전에 돌을 던지는 경우를 해결하지 못했다.
    - 몬스터가 사망했지만 오브젝트가 아직 사라지지 않은 상태에서 플레이어와 충돌하면 여전히 데미지를 입는 문제를 해결하지 못했다.
    - 현재 근접 공격은 태그로 충돌을 감지하여 데미지를 주고 애니메이션을 실행하도록 구현했지만, 공격 애니메이션으로 인해 팔의 위치가 변하는 점을 반영하지 못해, 실제로 주먹이 맞았을 때만 데미지를 입도록 하는 기능을 구현하지 못했다.
<br />

## 💁‍♂️ 프로젝트 팀원
|Front-End|Front-End|
|:--:|:--:|
|![](https://github.com/cjh5779.png?size=120)| |
|[최정환](https://github.com/cjh5779)|[김영준](https://github.com/youngjoon0405)|
