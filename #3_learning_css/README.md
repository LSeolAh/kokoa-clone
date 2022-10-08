### HTML에 CSS 적용 방법

1. 같은 HTML 파일에 넣기 → inline

- head Tag 안에 sytle Tag 작성

1. CSS와 HTML 분리 → external

- style.css 파일 생성 후 작성
- link Tag를 이용해 style.css와 연결하고 rel을 이용해 관계 적기

## CSS

- 가르키는 대상(Selector) 작성 후 중괄호{} 안에 원하는 속성 작성

```css
h1 {
  color: yellowgreen;
  text-decoration: underline;
  font-weight: 600;
  font-size: 20px;
}
address {
  text-align: center;
}
```

- text-aligin: center → 글자 가운데 정렬

### CSS; Cascading style sheets

- cascading: 연속
- 브라우저가 CSS 코드를 읽을 때 위에 있는 코드부터 차례대로 읽음
  → 속성을 겹치게 지정하면 결국 마지막 코드가 지정한 것으로 됨

## Box(Block)

- 옆에 아무 것도 올 수 없음
- 높이와 너비 존재
- div
- header
- footer
- address
- etc.

### 속성

1. margin: box의 border 밖에 있는 공간

- margin값을 1개
  - margin: 상 하 좌 우
- margin값을 2개
  - margin: (상/하), (좌/우)
- margin값을 3개
  - margin: 상, (좌/우), 하
- margin값을 4개
  - margin: 상, 우, 하, 좌

## inline

- 높이와 너비 존재 x
- span
- a(link)
- image
- etc.

## display

- inline ↔ block 변경 가능
