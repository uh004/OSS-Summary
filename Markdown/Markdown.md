# Markdown이란?

**마크다운이란 2004년 존그루버가 만든 텍스트 기반의 마크업 언어이다. 쉽게 읽고 쓸 수 있으며 HTML로 변환도 가능해 간편하다. 단 모든 HTML을 지원하지는 않는다. 작성법은 특수기호와 문자를 이용하며, 문법이 간단한 편이라 웹에서도 빠르게 컨텐츠를 작성할 수 있고 읽기도 좋다. 마크다운이 많이 쓰이기 시작한 때는 GitHub가 생겨난 후 부터이다. 깃허브의 원격저장소에 관한 정보를 기록하고 알려주는 README는 마크다운 언어로 쓰인다. 이를 기점으로 온라인 게시물에도 마크다운 언어를 많이 사용하기 시작했다.**

### 장점
- 배우기가 정말 쉽고 직관적이다.
- Text로 저장 후 HTML으로의 변환이 가능하다.변환을 지원하는 도구나 Eco(생태계)가 매우 많다.
- Text로 저장하기 때문에 Git을 통한 버전관리가 가능하고 용량이 적어 보관이 용이하다.

### 단점
- 유일한 단점은 표준이 없다. 핵심 문법을 제외하고는 에디터에 따라 결과물이 달라질 수 있다.
- 모든 HTML 마크업을 대신하지 못한다.

## Markdown태그설명
### 제목(header)
```
<h1> ~ <h6> 까지 제목 표현 방법
# 가나다라마바 1
## 가나다라마바 2
### 가나다라마바 3
#### 가나다라마바 4
##### 가나다라마바 5
###### 가나다라마바 6
```
# 가나다라마바 1
## 가나다라마바 2
### 가나다라마바 3
#### 가나다라마바 4
##### 가나다라마바 5
###### 가나다라마바 6
### 강조(emphasis)
```
*i love you*  이탤릭체
_i love you_ 

**i love you** 강조
__i love you__  

*i **love** you*
```
*i love you*  <br>
_i love you_  <br>

**i love you**  <br>
__i love you__  <br>

*i **love** you* <br>
### 목록(list)
```
순서있는 목록
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째
```
순서없는 목록
* red
  * green
    * blue

+ red
  + green
    + blue

- red
  - green
    - blue
```
* red
  * green
    * blue

+ red
  + green
    + blue

- red
  - green
    - blue
### 링크(links)
```
[GitHub](http://github.com "깃허브")
[naver](http://naver.com "네이버")
```
[GitHub](http://github.com "깃허브") <br>
[naver](http://naver.com "네이버")

### 이미지(images)
```
마크다운 형식
![다운로드sdfd](https://user-images.githubusercontent.com/105197524/195865824-8d5c57c1-342c-469b-ab44-890d1d2680dc.jpg)
태그 형식
<img src="https://user-images.githubusercontent.com/105197524/195865835-d5d8b25a-374f-43dd-91bf-071aa6efc398.jpg"  width="700" height="370">
```

![다운로드sdfd](https://user-images.githubusercontent.com/105197524/195865824-8d5c57c1-342c-469b-ab44-890d1d2680dc.jpg) <br>

<img src="https://user-images.githubusercontent.com/105197524/195865824-8d5c57c1-342c-469b-ab44-890d1d2680dc.jpg"> <br>

### 테이블(Table)
```
테이블 생성

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9
```

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9

## 인용 상자(Blockquotes)
```
how are you: 
> welcome to github
> right now
```
how are you: 
> welcome to github <br>
> right now

## 체크 박스(check box)
```
- [x] Fly on the Wall (*)
- [ ] Down in the Cockpit
- [x] English Roundabout (*)
- [x] Snowman
```
- [x] Fly on the Wall (*)
- [ ] Down in the Cockpit
- [x] English Roundabout (*)
- [x] Snowman

## 수평선(hr)
```
--- 
*** 
___
```
--- 
*** 
___

# 정리
**마크다운은 기본문법만 알고있다면 일반 텍스트편집기에서도 손쉽게 작성이 가능한 마크업언어다. 현재 다양한 도구와 플랫폼에서 지원하고 있기 때문에 더욱 손쉽게 스타일적용된 문서를 작성할 수 있어 점점 널리 사용되고 있다.**

<a href="https://www.markdownguide.org/cheat-sheet/">참고 자료</a>

