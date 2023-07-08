# CSS
>스타일을 담당

## 선택자
* `특정단어{명령}` : 특정 단어에 해당하는 부분 명령시 사용
```
li{
            color:red;
            text-decoration:underline;
        }
# 안에 두 문장 이상이 들어갈 경우 ; 으로 구분
``` 
* `id="값"`, `#값{명령}` : 하나만 바꾸고 싶은 경우 (#붙이기)
* `.class="명령"` : 그룹핑된 것들 명령하기 (id:주민등록번호, class:그룹) (. 붙이기)
* `ul li{명령}` : ul밑의 li에 명령
* `값{border:1px} solid red` : 테두리와 형태
* `ul>li{명령}` : ul태그 바로 밑에 있는 li에 명령
* `ul,ol` : 같은 명령어일 경우 , 으로 연결 가능
* `active{color:000;}` : 마우스를 누를 경우의 명령어
* `hover{color:000;}` : 마우스를 올려놓을 경우의 명령어(CSS는 명령이 중복 될 경우 뒷쪽의 명령을 따름)
* `focus{명령}` : 선택된 경우의 명령어
* `apple:not(.small)` : apple중 클래스 값이 small이 아닌 것
* +`<div></div>` : 순수 컨테이너로서 아무것도 표현하지 않는다. 다른 요소를 여럿 묶어 class나 id속성으로 꾸미기 쉽도록 돕거나 특정 구역이 다른 언어임을 표시한다.(lang속성 사용)

## 속성
* **font-size**
단위: px & em & rem (사용자가 브라우저의 글꼴 크기를 키웠을 때 px:바뀌지 않음, rem:바뀜)
* **color**
이름 : color name & hex & rgb (색갈 지정 방법)
* **text-align**
>텍스트 정렬 방법
`text-align: center, light, reft, justify`
* **font**
1. ##### font-family
>글꼴 지정 방법
`font-family: 폰트이름;` +폰트에 따라 뒤에 monospace, serif... 입력
2. ##### font-weight
>글꼴 두께
`font-weight: bold`
3. ##### font-height
>행 사이의 간격
`font-height: 2`
4. ##### font
>위의 내용을 한번에 작성
`font:(weight) (size)/(height) (family)`
* **web font**
1. 폰트 웹에서 폰드 다운 
2. head태그에 주소 넣기
3. 폰트 이름에 맞게 font-family속성 사용


## 중요 요소
`!important` : 이 명령문장을 우선시해라라는 의미

## css를 이용해 html 엘리먼트 위치변경
1. display
 * block : 위아래로 쌓임
 * inline : 왼쪽에서 오른쪽으로 정렬되는 성질

2. position
 * static : 기본적으로 가지는 값
 * absolute : 기준점에 따라 배치 가능, 상위 엘리먼트 값을 기준으로 가짐
 * relative : 원래 자신이 위치할 곳을 기준
 * fixed : 화면을 기준으로하여 위치 지정

3. float, clear
 * float : 지정된 엘리먼트를 띄우는 효과 (Z축으로)
 * clear : float을 감지하지 않도록 하는 방법
