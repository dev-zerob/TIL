## CSS Selector

선택자란 `선택을 해주는 요소`입니다. 이를 통해 특정 요소들을 선택하여 스타일을 적용할 수 있습니다.

<br />


### 모든 요소를 지정
```css
  * {
    /* 모든 요소에 스타일 지정 */
  }
```

### 특정 태그를 지정
```css
  ul {
    /* 모든 ul 태그에 스타일 지정 */
  }
  ul li {
    /* ul 태그 하위가 li 태그인 요소에 스타일 지정 */
  }
```

### 특정 ID를 가진 요소를 지정
```css
  #fancy {
    /* fancy라는 ID를 가진 요소에 스타일 지정 */
  }

  #fancy span {
    /* fancy라는 ID를 가진 요소의 하위가 span 태그인 요소에 스타일 지정 */
  }
```

### 특정 class를 가진 요소를 지정
```css
  .small {
    /* small라는 class를 가진 요소에 스타일 지정 */
  }
  div.small {
    /* div태그 중 small라는 class를 가진 요소에 스타일 지정 */
  }
```

### 2개의 요소를 지정
```css
  ul, ol {
    /* ul과 ol 태그에 스타일 지정 */
  }
```

### 인접한 요소를 지정
```css
  div + span {
    /* div에 인접한 span 태그에 스타일 지정 */
  }
```

### 두 개의 요소 사이에 있는 요소를 지정
```css
  div ~ button {
    /* div 태그와 button 사이에 있는 요소에 스타일 지정 */
  }
```

### 자식 선택자에 요소를 지정
```css
  div > span {
    /* div 태그를 부모로 가진 span 태그에 스타일 지정 */
  }

  ul > li:first-child {
    /* ul 태그를 부모로 가진 첫번째 li 태그에 스타일 지정  */
  }

  ul li:only-child {
    /* ul 태그를 부모로 가진 외동 li 태그에 스타일 지정 */
  }

  ul li:last-child {
    /* ul 태그를 부모로 가진 마지막 li 태그에 스타일 지정 */
  }

  ul li:nth-child(2) {
    /* ul 태그를 부모로 가진 두번째 li 태그에 스타일 지정 */
  }

```

### 선택한 요소의 상태에 따른 지정
```css
  span:first-of-type {
    /* span 태그 중 첫번째 요소에 스타일 지정 */
  }

  span:last-of-type {
    /* span 태그 중 마지막 요소에 스타일 지정 */
  }

  span:nth-of-type(2) {
    /* span 태그 중 두번째 요소에 스타일 지정 */
  }

  span:nth-of-type(2n+1) {
    /* span 태그 중 2n+1째 요소에 스타일 지정 */
  }

  span:nth-of-type(odd) {
    /* span 태그 중 홀수 요소에 스타일 지정 */
  }

  span:nth-of-type(even) {
    /* span 태그 중 짝수 요소에 스타일 지정 */
  }
```

### 빈 요소를 지정
```css
  div:empty {
    /* 빈 div 요소에 스타일 지정 */
  }
```

### 아닌 요소를 지정
```css
  div:not(.small) {
    /* div 태그 중 class가 small이 아닌 요소에 스타일 지정 */
  }
```

### 속성으로 요소를 지정
```css
  a[href] {
    /* a태그 중 href 속성이 존재하는 요소에 스타일 지정 */
  }

  a[href="naver.com"] {
    /* a태그 중 href 값이 "naver.com"인 요소에 스타일 지정 */
  }

  a[href^="naver"] {
    /* a태그 중 href 값이 "naver"로 시작하는 요소에 스타일 지정 */
  }

  a[href$=".com"] {
    /* a태그 중 href 값이 ".com"로 끝나는 요소에 스타일 지정 */
  }

  a[href*="ave"] {
    /* a태그 중 href 값이 "ave"를 포함하는 요소에 스타일 지정 */
  }
```

<br />
<br />


> **출처**
>
> - [CSS Dinner ](https://flukeout.github.io/)
>