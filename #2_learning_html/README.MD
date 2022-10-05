<aside>
💡 goolge에 검색 시 mdn키워드를 붙여서 검색하기 추천
→ Mozilla developer Network 사이트로 안내

</aside>

[HTML&colon; Hypertext Markup Language | MDN](https://developer.mozilla.org/ko/docs/Web/HTML)

## HTML Tag

- 어디서부터 어디까지가 무엇인지 얘기해 주는 것
- tag를 text로 넣음 → title, link 등이 될 수 있음
- <h1>태그 열기
- </h1>태그 닫기

### H1 Tag

- header number 1
- <h1>Hello this is my website!</h1>
    
    → Hello this is my website!만 출력


### List Tag

- ol(ordered list)
  - 순서가 있는 목록
  - 숫자로 정렬됨
- ul(unordered list)
  - 순서가 없는 목록
  - -으로 나옴

### a Tag

- anchor(닻)
- 다른 링크로 이동하게 해줌
- a태그에는 다른 부가적인 정보(attribute) 필요
  - href (HTTP reference ; hyperlink refernce):
  - target
    - `_self` → 기본값 : 같은 페이지 내에서 열림
    - `_blank` → 새로운 탭으로 열림

### image Tag

- 이미지 넣는 태그
- img 태그는 자체 닫기 태그
  - src = “”를 통해서 이미지 주소 or 파일 경로 넣기

## HTML 규칙

<!DOCTYPE *html*> → 필수; 브라우저에게 html 문서라고 알려주는 것

<html></html> → 이 태그 안에 넣는 것이 html 코드가 됨

- <html lang=””> → 검색엔진에게 사용되는 주된 언어가 무엇인지 알려줌

<head></head> → 웹사이트의 환경 설정; 외부적으로 보여지지 않음

- <title></title> → 웹페이지 제목 설정
- <meta></meta> → 부가적인 정보; 제목 밑에 나오는 설명(content, name attribute 가짐)
    - content: 설명 내용
    - name: 검색 했을 때 제목 밑에 나오는 설명
- <meta charset="utf-8"/> → 브라우저에 텍스트를 어떻게 그려주는지 말해줌; 글씨 안깨짐
- <link />
    - rel(relationship) → shortcut icon 입력 시 title의 아이콘을 가리킴
    - sizes → 아이콘의 사이즈 설정
    - href → 아이콘의 경로 설정
- <meta property="og : "> → 콘텐츠의 요약 내용이 SNS에 게시되는데 최적화된 데이터로 가지고 갈 수 있도록 설정(og → 카톡)
    - title, type, url, image, description …

<body></body> → 사용자가 볼 수 있는 content를 보여줌

- <abbr title=””></abbr>
  - <p> 태그 안에 abbreciation에 title인 attribute 작성
  - 약칭의 의미는 title에 작성; 약어는 content에 넣기
  - 마우스를 해당 글자에 올려주면 title에 작성한 text가 나옴
    ```html
    <p>My name is <abbr title="LSeolAh">LSA</abbr></p>
    ```

### form Tag

- <input /> → 입력받는 칸
  - type → input의 유형 결정
    - color → 색 선택
    - password → \*\*\*로 나타남
    - text : 입력한대로 출력
    - submit → 버튼 역할; form 정보 전송
  - placeholder → input값에 무엇을 입력해야하는지에 대한 정보 제공
  - value → 내용 바꿔줌
    - type = “submit” → submit이란 이름으로 버튼 생성
  - disable → input 기능 안됨
  - require → input 검증; DB의 NN
  - minlength → input 최소 길이 지정

### label Tag

- label은 input과 함께 사용
- <label for=””> → for 값은 <input id=””>의 id와 동일한 값이여야 함
- id→ 태그 당 하나의 id만 가져야 함; 고유식별자

### semantic Tag

- 직관적으로 무엇인지 알 수 있는 태그
- header
- main
- footer

### non-semantic Tag

- div
- span
