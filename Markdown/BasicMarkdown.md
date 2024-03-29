# 기초적인 마크다운 문법

[목록으로 돌아가기](/README.md)

## 1. 마크다운이란?

쉽고 빠르게 보기 좋은 HTML 문서를 작성할 수 있는 문법. 깃허브([https://github.com](https://github.com)) 저장소에 관한 정보를 기록하는 용도로 자주 쓰인다.

## 2. 마크다운 문법 정리(하면서 공부하기)

### 2.1 헤더 Headers

* 문서의 제목

```txt
제목
===== (H1)

or

# 제목 (H1)
```

* 문서의 소제목

```txt
소제목
----- (H2)

or

## 소제목 (H2)
### 소제목 (h3)
.
.
.
###### 소제목 (H6)
```

####### H7은 지원하지 않는다

`=-`와 `#` 중 한 가지만 사용하는 것이 권장된다.

### 2.2 인용구 BlockQuotes

`>` 를 사용해 작성한다.

> 이것은 인용구 입니다.
>> 인용구 들여쓰기.
>>> 한 번 더.
>>>> 한 번 더...
>>>>> 또?
>>>>>> `텍스트`
>>>>>>> 내부에서 마크다운 문법을 사용 가능하다.

### 2.3 목록 Lists

#### 2.3.1 순서가 있는 목록

```txt
1. 첫 번째
2. 두 번째
3. 세 번째
```

1. 첫 번째
2. 두 번째
3. 세 번째

#### 2.3.2 순서가 없는 목록: `*`, `+`, `-` 사용

```txt
* 목록1
  * 목록 들여쓰기
    * 한 번 더 들여쓰기
      * 한 번만 더...

+ 사용법은 같다
  + 들여쓰기도 가능
  
- 이하동문
  - Yo!
```

* 들여쓰기를 하면
  * 모양이
    * 바뀐다

마찬가지로 한 종류의 기호만 사용하는 것이 권장된다.

### 2.4 코드 Codes

#### 2.4.1 들여쓰기

4개의 공백 또는 하나의 탭으로 들여쓰기를 하면 들여쓰지 않은 행까지 코드블록이 된다.

```txt
이것은 일반 문장입니다.

    여기는 코드블록입니다.

코드 블록 끝.
```

#### 2.4.2 `<pre><code>{code}</code></pre>` 사용하기

```txt
<pre>
<code>
def function(a, b):
    return a+b
</code>
</pre>
```

<pre><code>
def function(a, b):
    return a+b

</code></pre>

#### 2.4.3 코드블록코드(```) 사용하기

<pre><code>
```python
def function(a, b):
    return a+b
```
</code></pre>

```python
def function(a, b):
    return a+b
```

### 2.5 수평선 Horizontal Rules

수평선을 만들기 위해서는 최소 3개의 *, -, _가 필요하다.

```txt
***
* * *
_____
```

***

----

_____

마찬가지로 한 종류만 사용하는 것이 권장된다.\

### 2.6 링크

#### 2.6.1 외부링크

```txt
[링크 텍스트](URL "마우스오버 텍스트")

[구글](https://www.google.com/ "구글 메인 페이지")
```

[구글](https://www.google.com/ "구글 메인 페이지")

#### 2.6.2 자동링크

```txt
단순 URL이나 이메일 주소는 <>를 사용해서 간단하게 표기 가능하다.
<https://www.google.com/>
<id@gmail.com>
```

<https://www.google.com/>

<id@gmail.com>

```txt
<> 없이도 URL은 자동으로 링크가 걸리지만, ``으로 감싸주면 일반 텍스트가 된다.
`https://www.google.com/`
```

`https://www.google.com/`

#### 2.6.3 깃허브 파일 참조하기

```txt
[링크 텍스트](파일경로)
주의: 파일명에 띄어쓰기를 사용하지 않아야 한다.

[Link Sample.md](LinkSample.md)
```

[Link Sample.md](LinkSample.md)

#### 2.6.4 문서 내부 헤더 참조하기

```txt
[링크 텍스트](#헤더 id)
[2.6 링크](#26-링크)
```

[2.6 링크](#26-링크)

### 2.7 강조

```txt
*기울이기*
_기울이기_
**굵게**
__굵게__
~~취소선~~
```

*기울이기*

_기울이기_

**굵게**

**굵게**

***서로 조합도 가능***

~~취소선~~

### 2.8 표

```table
|분류1|분류2|분류3|
|-----|-----|-----|
|A|B|C|
```

|분류1|분류2|분류3|
|-----|-----|-----|
|A|B|C|

`|`와 `-`를 사용해서 표를 만들 수 있다.
