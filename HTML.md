# HTML
## 태그
### 전체 감싸기
`<html>abc</html>`
### 헤드
`<head>abc</head>`로 묶어줌
#### 1. 파일 탭 이름
`<title>abc</title>`
#### 2. 글씨 깨질 경우
`<meta charset="utf-8">`
#### 3. doctype - 가장 위에 위치
`<!DOCTYPE html>`

### 문단
`<body>abd</body>`로 묶어줌
#### 1. 제목
`<h1></h1>`
#### 2. 리스트 형식 나열
`<ul></ul>`
#### 3. 숫자 리스트 형식 나열
`<ol></ol>`
#### 4. 링크
`<a></a>`
#### 5. 굵은 글씨
`<strong></strong>`

## 속성
#### 1. 링크
`href="http:~`
#### 2. 새창에 열기
`target="_blank`
#### 3. 툴팁
`title="설명"`


## 중요태그 
#### 1. 단락&줄바꿈- p태그
`<p>한 문단</p>`
#### 2. 줄 간격 조정- br태그
단락 뒤 `<br>` (띄우고 싶은 만큼 중복 입력)
#### 3. 이미지 태그 -img태그
`<img src="이미지 파일 주소" width="픽셀크기" height="높이" alt="대체제 이름">`


## 표
#### 표 태그 -전체 묶기
`<table></table>`
#### 표 칸 태그
`<td>표 칸 하나의 값</td>`
#### 표 행 태그
`<tr>같은 행</tr>
#### 테두리 속성
`border="굵기에 대응하는 숫자"`

#### 표 헤드
`<thead></thead>`
#### 표 바디
`<tbody></tbody>`
#### 표 중요 단어
##### <td>대신 `<th>`
표 가장 밑 행
`<tfoot>같은 행</tfoot>`

#### 표 병합
수직 병합 - 병합 첫번째 칸 태그에 속성 `rowspan="병합 행 갯수"` 추가
수평 병합 - 병합 첫번째 칸 태그에 속성 `colspan="병합 열 갯수"` 추가
**속성이 적힌 대표 칸 제외 나머지 삭제 필요**


## form
> 사용자가 선택한 것을 서버로 전송하는 역할
>  submit 버튼 입력 후 보낼 주소 입력 태그
>  속성 `action="UIL"`사용
#### input
> 사용자에게 입력받게하는 태그
>  속성 `type="ex: text"`을 필요
>  +type이 비밀번호 형식으로 입력 필요 `password`
>  +서버 전송 필요시 `submit` , 전공(제출) 버튼 이름 변경 시 `value=""`사용
>  +안내문 입력칸에 넣을 필요시 `placehodler="id를 입력해주세요"'
#### 입력 값 control하기
> input 태그에 속성 `name=""`사용
#### 입력 칸 기본 문구
>input 태그에 속성 `value="~~"`사용
#### 여러 줄 입력
>`<textarea></testarea>`
> + 속성 : 입력값 칸 지정 `cols=", "``rows=""`
> *입력 칸 기본 문구 지정 시 `<textarea>기본문구</testarea>`형식으로 작성*

## 선택하기
##### 전체 태그`<select></select>`
>선택 옵션 이름 속성 `name=""`사용
##### 옵션 태그`<option></option>`
>전송되는 데이터 네임 바꾸기 속성 `value=""`사용
##### 다중 선택 시 
>속성`multiple`사용
+`type="reset"`시 재설정 버튼

### 여러개, 복수 선택하기- radio 버튼&checkbox
#### radio 버튼 -name별로 여러개 선택
`<input **type="radio"** name="" value="">`
>name값이 같은것끼리 선택 가능
#### checkbox - 여러개 선택
`<input **type="checkbox"** name="" value="">`
##### +기본 체크 표시
속성 `checked`사용

### button
> 자바스크립트와 함께 사용

## hidden filed
>화면상에 보이지 않지만 주소로 전송되는 것
`type="hidden"`

## lable
>무언가의 이름표
```
<lable for="id_txt">text</lable>
<input id="id_txt" type="text" name="id" value="default value">
```

## method
>전송 방식
##### post 방식
from 태그에 `method="post"`속성 부여
>UIL이 아닌 방식으로 정보를 숨겨서 전송


## upload - php파일연과
>선택 파일 전송&서버에 장
```