## Animate-All-The-Things-

#### 1. animation-delay
animation 속성은 적용되는 시점부터 바로 동작하게 됩니다. <br/>
animation-delay는 원래 시작되는 시점에서부터 일정시간만큼 대기했다가 시작하게 하는 속성입니다. <br/>
일반적으로 속성값은 양수를 사용합니다. 하지만 음수를 넣을 경우, delay 없이 시작하지만 애니메이션의 동작지점이 절대값만큼 지난 시점부터 진행됩니다. <br/>

#### 2. 예시처럼 반복적으로 멈췄다가 다시 동작하게 하는 방법
animation-delay는 animation이 적용되는 첫 시점에만 적용됩니다. <br/>
따라서 예시처럼 멈췄다가 다시 동작하게하려면, animation이 동작하는 시간에 공백을 만들어 주면 됩니다. <br/>
예를 들어 1s 동안 animation을 진행한다면, 0.5s(50%)에 이미 동작을 완료하고 1s(100%)에는 완료된 동작을 유지(50%와 동일한 내용)하는 코드를 작성하는 방식입니다. <br/>

#### 3. transform
transform 속성을 이용하면, 요소를 돌리고, 늘리고, 이동하고, 비틀고 등 다양하게 변형할 수 있습니다. <br/>
예시처럼 회전시키려면 rotate, 늘리려면 scale 을 사용하면 됩니다. <br/>

#### 4. transform: translate(...)
translate의 경우 단순히 animation을 위한 움직임으로 사용할 수 있지만, 요소를 원하는 위치에 배치하기 위한 수단으로 사용할 수 있습니다. <br/>
특히 position: absolute; 인 요소를 부모의 정중앙에 배치하고자 할 경우에 사용할 수 있습니다. <br/>
absolute가 선언된 요소에 top: 50% 과 left: 50% 을 선언했을 때, 정중앙에 오는 것은 absolute 요소의 좌상단 꼭지점입니다. <br/>
여기에 transform: translate(-50%, -50%); 를 선언해주면, 요소의 크기를 기준으로 너비 50%, 높이 50% 만큼을 좌상으로 이동합니다. <br/>

#### 5. border-radius
border-radius 속성을 통해 요소의 꼭지점들을 곡선으로 만들 수 있습니다. <br/>
width와 height가 동일할 경우, border-radius에 50%를 입력하면 원이 만들어집니다. <br/>
또한, 네 꼭지점 중 한 곳을 제외한 세 곳에 border-radius를 적용함으로써 말풍선 모양의 박스도 구현할 수 있습니다. <br/>

### 결론
Animation과 관련된 여러 속성들을 이용하면 다양한 애니메이션 효과를 구현할 수 있습니다. <br/>
Transform은 꼭 animation과 함께 사용할 필요는 없습니다. 단독으로도 많이 활용될 수 있습니다. <br/>
