# markdown 문법 필기

## heading

* h1 -> `#` -> html `<h1>내용물</h1>`
* h2 -> `##`
* h3 -> `###`
* h4 -> `####`
* h5 -> `#####`
* h6 -> `######`

`ctrl` + `숫자` 로 전환 가능



## list

### unorderd list (순서가 없는 리스트)

`*` / `-`

* a
    * b
        * c
            * d
                * e
                    * f

1. java
2. python
   * django
   * sqlite
     1. 
     2. 
     3.
     4.

`<ul></ul>`

### ordered list (순서가 있는 리스트)

`숫자` + `.`

1. 순서가 있는 리스트 1
2. 순서가 있는 리스트2
    1. 순서가 있는 리스트 2의 1
        1. 순서가 있는 리스트 2의 1의 1

`<ol></ol>`



## text style

### bold

`**` 볼드`**`

`ctrl`+`b`

안녕하세요 **오지혜**입니다.



### italic

`*` 기울기`*`

`ctrl`+`i`

안녕하세요 *싸피*입니다.



* bold + italic
    * 안녕하세요 ***서울 9반***입니다.



## hyperlink

### link

`[텍스트](내가 가고 싶은 url)`

[구글](https://www.google.com)

[네이버](https://www.naver.com)

### img

`![대체 텍스트]( )`

![남산타워](https://thumb.tidesquare.com/tour/public/product/PRV3000000010/PRD3000822580/editor/20230803023524191_4bvAw.jpg)


### 수평선 
___

## Code Block

### inline code block

빽킷을 활용해서  인라인 코드 만들 수 있어요.

글 1, 글2 , 글3, `코드1`





### code block

빽킷을 세번 입력

```java
// TIL/intro1.java 주석

class sample {
    public static void main(String args[]){
        System.out.println("Hello Java");
    }
}
```

### code block 줄1개
`String text = "abcd"`





## Table

`|` bar을 이용

| 이름 | 학년 | 기수 | 전공 | 연락처 |
| ---- | ---- | ---- | ---- |--|
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |
|      |      |      |      |  |