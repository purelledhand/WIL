## Virtual DOM and Render in Browsers

이 글은 주요 FE 프레임워크 별 Virtual DOM을 기반으로 DOM manipulation 과정을 어떻게 최소화해 나가는지를 비교하기 위해 작성한 글이다.

#### 1. Common Concept

jQuery, Vanilla.js 는 DOM을 직접 조작하기 때문에 값이 변경될 때마다 전체 DOM이 모두 다시 repainting되는 반면, 고도화 된 현대 FE 프레임워크에서는 Virtual DOM을 통해 real DOM과 변경된 부분만 diffing하여 업데이트 하여 전체 DOM Manipulation 과정을 최소화한다.

먼저 브라우저에서 DOM이 렌더링 되는 과정은 다음과 같다.

#### DOM manipulation

1. **DOM Tree와 CSS를 머지한 후 빌드**

2. **Reflow**

   DOM의 레이아웃 수치 변경 시 영향을 받는 모든 노드의 스타일 수치를 다시 계산하여(Recalculate), 렌더 트리를 재생성하는 과정

3. **Repaint**

   Reflow에 의해 재생성된 렌더트리를 다시 그리는 과정

> 위에서 언급된 `reflow` 와  `repaint` 연산은 browser layout rendering operation 중 가장 무겁게 동작한다.

기존의 jQuery, Vanilla.js 는 DOM을 직접 조작하는데, DOM을 조작할 때마다 레이아웃 변화, 트리 변화 및 렌더링을 발생시켜서 매 조작이 위 DOM Manipulation 과정을 거치게 된다.

SPA 웹 프레임워크 (앵귤러, 리액트, 뷰)들은 이 문제를 Virtual DOM을 사용하여 해결하였다. 데이터 값에 변화가 일어나면 이를 Virtual DOM에 적용한 후 오프라인 DOM 트리에 적용시킨다. (오프라인 DOM 트리는 렌더링 되지 않기 때문에 연산 비용이 적다.) 이 후 모든 변화들을 적용시킨 후 real DOM과 diffing하여 변경된 부분만 update하여 DOM Manipulation 과정을 최소화한다.

여기까지가 SPA 웹 프레임워크에서 Virtual DOM을 이용하는 공통된 컨셉이다. 이 후로는 각 프레임워크 별로 어떻게 Reacivity를 적용하는 지, Key Concept에 대해서 정리한다.

#### 2. Vue

Vue에서 바인딩의 개념은 Virtual DOM과 데이터를 연결시킨다는 개념이다. Vue Instance 내의 data object는 Vue의 reactivity system에 연결되어 있는데, data object 내부 속성의 값이 변경되면 view가 re-render되어 Virtual DOM에 적용된다.

**Reactivity**

* Vue performs DOM updates asynchronously
* 

