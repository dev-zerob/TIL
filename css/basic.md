## CSS 란?

`Cascading Style Sheets`는 `HTML`, `XHTML`, `XML`와 같은 문서의 스타일을 꾸밀 때 사용하는 스타일 시트 언어입니다.

<br />


## Cascading
- Author Style (작성된 스타일)
- User Style (사용자가 적용하는 스타일) _ex) Dark Mode_
- Browser (브라우저에서 지정되는 스타일)

<br />


### padding vs margin
- margin : 콘텐츠의 밖의 여백
- padding : 콘텐츠의 안의 여백

<br />


### display
- block : 한 줄에 하나만 배치가 가능하며, 크기를 지정할 수 있습니다.
- inline : 한 줄에 들어갈 수 있는 영역 만큼 배치가 가능하며, 크기를 지정해도 내용의 사이즈에 맞춰 적용됩니다.
- inline-block : 크기를 지정할 수 있으며, 한 줄에 들어갈 수 있는 영역 만큼 배치가 가능합니다.

<br />


### position
- static : HTML에 정의된 순서대로 브라우저에 보여집니다. _(Default)_
- relative : 원래 있어야 하는 자리에서 상대적으로 배치가 가능합니다.
- absolute : 부모의 요소 기준에서 절대적으로 배치가 가능합니다. 
- fixed : 페이지 기준에서 절대적으로 배치가 가능합니다.
- sticky : 스크롤링을 하여도, 기존 자리에서 벗어나지 않고 Floating 됩니다.

<br />


### Flex Box
Container의 속성
- display : `flex` 값을 주어 flex box로 만들어야 합니다.
- flex-direction : 정렬 기준을 변경할 수 있는 속성입니다.
  - row : 왼쪽에서 오른쪽으로 정렬 _(Default)_
  - row-reverse : 오른쪽에서 왼쪽으로 정렬
  - column : 위에서 아래로 정렬
  - column-reverse : 아래에서 위로 정렬
- flex-wrap : 아이템들을 강제로 한줄 배치를 할 것인지 설정할 수 있는 속성입니다.
  - nowrap : 한 줄에 가득 차도 아이템들을 강제로 한 줄에 배치 _(Default)_
  - wrap : 한 줄에 가득 차면 아이템을 자동으로 다음 줄에 배치
- flex-flow : `flex-direction`과 `flex-wrap`을 한 번에 작성할 수 있도록 해주는 속성입니다.
- justify-content : 아이템들의 배치 기준을 변경할 수 있는 속성입니다.
  - flex-start : 시작점을 기준으로 정렬
  - flex-end : 끝점을 기준으로 정렬
  - center : 가운데 기준으로 정렬
  - space-around : 아이템 양 옆에 일정한 간격으로 추가하여 정렬
  - space-evenly : 아이템의 간격을 모두 일정하게 정렬
  - space-between : 양 끝 간격을 제외한 아이템 간의 간격을 모두 일정하게 정렬
- align-items : 아이템의 정렬 기준을 변경할 수 있는 속성입니다.
  - baseline : 가장 큰 높이의 아이템 기준으로 가운데 정렬
- align-content : `justify-content`과 반대되는 축의 배치 기준을 변경할 수 있는 속성입니다.

Item의 속성
- flex-grow : Item의 크기 비율을 변경할 수 있는 속성입니다. _(default: 0)_
- flex-shrink : Item의 크기가 줄어드는 비율을 변경할 수 있는 속성입니다. _(default: 0)_
- flex-basis : Item의 크기를 퍼센트로 변경할 수 있는 속성입니다. _(default: auto)_
- flex : `flow-grow`, `flex-shrink`, `flex-basis`를 한 번에 작성할 수 있도록 해주는 속성입니다.
- align-self : Container의 반대 축 정렬을 벗어나 정렬하고 싶을때 사용하는 속성입니다.

<br />


### `%` vs `vh`
- % : 부모 요소의 (넓이,높이) 100% 만큼 (넓이,높이) 설정
- vh : 부모 상관없이 viewport의 100% 만큼 (넓이,높이) 설정

<br />
<br />


> **출처**
>
> - [CSS - Youtube 드림코딩 by 엘리](https://www.youtube.com/watch?v=gGebK7lWnCk&list=PLv2d7VI9OotQ1F92Jp9Ce7ovHEsuRQB3Y&index=8)
>