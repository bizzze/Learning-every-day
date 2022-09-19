# 2022.09.19 Learning MardDown Syntax

# Headers

# This is and H1

## This is an H2

### it is like html <h> tag / using

# BlockQuote(인용문)

// using >

인용문(BlockQuotes)

> 남의 말이나 글에서 직접 또는 간접으로 따온 문장.
>
> > _(네이버 국어 사전)_

> This is a first blockquote
>
> > this is a second blockquote

# List.

// Order list (number) <br>
// using number and dot. <br>
// 어떤 번호를 입력해도 순서는 내림차순으로 정의됨. <br>

-> 지금 사용하는 1. 2. 3. 방식이 order list 방식. <br>

// disorder list (using +,-,\*) <br>

- 빨강
- 녹색
- 파랑

# Code

// 4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 <br>
// 변환되기 시작하여 들여쓰지 않은 행을 <br>
// 만날 때까지 변환이 계속됨 <br>

This is a normal paragraph :

    This is a code block.

end code block.
// 꼭 한 줄 띄어줘야 함!!

## Code block

Using

<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>

or

```java (깃헙에서는 시작점에 사용 언어 선언해서 문법강조가 가능!!)
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
```

# 수평선 `<hr/>`

---

# link `<a>`로 변환됩니다.

<참조링크>

[linkname][url]  
[linkname][url "you can write description of link!"]  
[linkname][my folder path] -> 상대적 참조

---

[Dribble][dribble link]  
[Github][1]  
문서 안에서 [참조링크]를 그대로 사용할 수 있다!

[참조링크]: https://naver.com "네이버로 이동합니다~!"
[github]: https://github.com
[dribble]: https://naver.com

다음과 같이 문서 내 일반 URL이나 꺾쇠 갈호(`<>`, Angle Brackets)안의 URL은 <br>
자동으로 링크를 사용합니다!

구글 홈페이지 : https://google.com <br>
네이버 홈페이지: <https://naver.com>

# img

image는 위 링크 양식 앞에 !만 붙입니다!

[![naver][https://search.pstatic.net/common/?src=http%3a%2f%2fcafefiles.naver.net%2fmjaxnzaxmjzfmtew%2fmdaxndg1ndezmzy3ndgw.6owkgt59a6llptykwuwdg0dheaa84xwru12fxzagy_mg.bmbuhpf3m8izalb5rv9iuhxd1nc5lbpewuvh5pjxnw4g.jpeg.master_of_travel%2fandroid_5.png&type=ofullfill340_600_png](https://dict.naver.com/search.dict?dicQuery=plaintext&query=plaintext&target=dic&ie=utf8&query_utf=&isOnlyViewEE=)

이미지 코드를 링크코드와 같이 묶을 수도 있어요! <br>
마치 `<div><img src="#"/><a href="#"></a></div>`

# code 강조

-> 해당 코드 tag를 썼다 등을 강조했을 때, 설명할 때 ``을 사용하면 유용

## inline code 강조

-> `background` 이런 식으로 강조 가능하다.

# table

-> `<table>` tag로 변환된다.<br>
-> 헤더 셀을 구분할 때, 3개 이상의 `-`(desh) 기호가 필요하다.<br>
-> 헤더 셀을 구분하면서 `:` (colons) 기호로 셀(열/칸) 안에 내용을 정렬할 수 있다.<br>

| 값         | 의미                                           | 기본값   |
| ---------- | :--------------------------------------------- | :------- |
| `static`   | 유형(기준) 없음 / 배치 불가능                  | `static` |
| `relative` | 요소 **자신**을 기준으로 배치                  |          |
| `absolute` | 위치 상 **_부모_(조상)요소** =를 기준으로 배치 |          |
| `fixed`    | **브라우저 창**을 기준으로 배치                |          |

# 수정본

**list는 markdown 문서로 보면 inner 요소로 보인다.**<br>
그러니까, 단락은 h1이나 강조로 나누고, 안에 item을 정리할 때, list를 쓰자!

- h1 양식 사용 시, 띄어쓰기!!
