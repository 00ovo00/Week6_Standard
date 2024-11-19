# Week6_Standard
<details>
 <summary><b> Q1. 심화주차 1-3강 ( UI 만들기 ) </b></summary>
    <div markdown="1">
    <ul>

**확인 문제 : 강의를 듣고, 강의 내용을 다시 점검하는 문제를 풀어봅시다.**

<aside>
🧠 UI의 앵커와 피벗에 대해서 세팅하는 19강의 강의 자료를 다시 확인해보시고, 
아래 퀴즈를 풀어보세요!

</aside>

**[🅾️❎퀴즈]**

- 앵커와 피벗은 같은 기능을 한다. (O/X)
    
    > X
    앵커는 부모 요소에 대한 해당 UI의 상대적 위치를 나타내며 화면의 해상도와 크기에 따라 동적으로 대응할 수 있게 한다.
    피벗은 해당 UI 자체에 대한 값으로 UI 크기가 변하거나 회전할 때의 기준점을 설정하는 역할을 한다.
    > 
- 피벗을 왼쪽 상단으로 설정하면, UI 요소는 화면의 왼쪽 상단을 기준으로 위치가 고정된다. (O/X)
    
    > X
    피벗은 UI 요소의 자체의 기준점이므로 부모 요소에 대한 상대적 위치를 반영하지 않는다. UI 요소를 화면 왼쪽 상단에 고정하려면 앵커를 사용해야 한다.
    > 
- 피벗을 UI 요소의 중심에 설정하면, 회전 시 UI 요소가 중심을 기준으로 회전한다. (O/X)
    
    > O
    크기나 회전의 기준점인 피벗이 UI 중심에 있으므로 회전 시 중심을 기준으로 회전하게 된다.
    > 

**[🤔 생각해보기]**

- 게임의 상단바와 같이 화면에 특정 영역에 꽉 차게 구성되는 UI와 화면의 특정 영역에 특정한 크기로 등장하는 UI의 앵커 구성이 어떻게 다른 지 설명해보세요.
    
    > Panel(기본 생성 시 화면 전체에 stretch)의 경우 앵커가 부모 오브젝트 기준으로 설정된다. Image(기본 생성 시 해당 오브젝트 중심)의 경우 앵커가 UI 요소 중심으로 설정된다. 화면 크기가 변동 될 때 화면 특정 영역에 꽉 차게 구성되는 UI는 변동 된 화면 크기에 맞추어 크기가 변동 된다. 특정 크기로 등장하는 UI는 화면 앵커가 자신의 중심에 있으므로 변동 되지 않는다.
    > 
- 돌아다니는 몬스터의 HP 바와 늘 고정되어있는 플레이어의 HP바는 Canvas 컴포넌트의 어떤 설정이 달라질 지 생각해보세요.
    
    > Canvas의 RenderMode 설정을 다르게 한다.
    돌아다니는 몬스터의 HP 바는 world 좌표 기준으로 계속 변하므로 World Space로 설정한다. 고정되어있는 플레이어의 HP바는 world 공간과 무관하게 화면에 바로 그려져도 상관 없으므로 ScreenSpace Overlay로 설정한다.
    >
  </ul>
  </div>
</details>
