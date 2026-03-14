---
title: 'Markdown 스타일 가이드'
description: 'Astro에서 Markdown 콘텐츠를 작성할 때 사용할 수 있는 기본 Markdown 구문 샘플입니다.'
excerpt: 'Markdown을 사용하여 텍스트를 서식 지정하는 방법을 배워보세요. 제목, 단락, 이미지, 인용구 등 다양한 요소를 다룹니다.'
pubDate: 'Mar 14 2026'
heroImage: '../../assets/Markdown-mark.png'
---

Astro에서 Markdown 콘텐츠를 작성할 때 사용할 수 있는 기본 Markdown 구문 샘플입니다.

## 제목

다음 HTML `<h1>`—`<h6>` 요소는 섹션 제목의 6단계를 나타냅니다. `<h1>`은 가장 높은 섹션 레벨이고 `<h6>`은 가장 낮습니다.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## 단락

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## 이미지

### 구문

```markdown
![대체 텍스트](./이미지의/전체/또는/상대/경로)
```

### 출력

![블로그 플레이스홀더](../../assets/blog-placeholder-about.jpg)

## 인용구

인용구 요소는 다른 출처에서 인용된 콘텐츠를 나타내며, 선택적으로 `footer` 또는 `cite` 요소 내에 인용 출처를 포함할 수 있고, 주석이나 약어와 같은 인라인 변경 사항을 선택적으로 포함할 수 있습니다.

### 속성 없는 인용구

#### 구문

```markdown
> Tiam, ad mint andaepu dandae nostion secatur sequo quae.  
> **참고** 인용구 내에서 _Markdown 구문_을 사용할 수 있습니다.
```

#### 출력

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.  
> **참고** 인용구 내에서 _Markdown 구문_을 사용할 수 있습니다.

### 속성이 있는 인용구

#### 구문

```markdown
> 메모리를 공유하여 통신하지 말고, 통신하여 메모리를 공유하라.<br>
> — <cite>Rob Pike[^1]</cite>
```

#### 출력

> 메모리를 공유하여 통신하지 말고, 통신하여 메모리를 공유하라.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: 위 인용구는 Rob Pike의 [강연](https://www.youtube.com/watch?v=PAAkCSZUG1c)에서 발췌한 것으로, 2015년 11월 18일 Gopherfest에서 했습니다.

## 표

### 구문

```markdown
| 이탤릭   | 굵게     | 코드   |
| --------- | -------- | ------ |
| _이탤릭_ | **굵게** | `코드` |
```

### 출력

| 이탤릭   | 굵게     | 코드   |
| --------- | -------- | ------ |
| _이탤릭_ | **굵게** | `코드` |

## 코드 블록

### 구문

새 줄에 3개의 백틱 ```을 사용하고 스니펫을 작성한 후 새 줄에 3개의 백틱으로 닫습니다. 언어별 구문 강조를 위해 첫 3개의 백틱 뒤에 언어 이름을 한 단어로 작성하세요. 예: html, javascript, css, markdown, typescript, txt, bash

````markdown
```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```
````

### 출력

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

## 목록 유형

### 순서 있는 목록

#### 구문

```markdown
1. 첫 번째 항목
2. 두 번째 항목
3. 세 번째 항목
```

#### 출력

1. 첫 번째 항목
2. 두 번째 항목
3. 세 번째 항목

### 순서 없는 목록

#### 구문

```markdown
- 목록 항목
- 다른 항목
- 그리고 다른 항목
```

#### 출력

- 목록 항목
- 다른 항목
- 그리고 다른 항목

### 중첩 목록

#### 구문

```markdown
- 과일
  - 사과
  - 오렌지
  - 바나나
- 유제품
  - 우유
  - 치즈
```

#### 출력

- 과일
  - 사과
  - 오렌지
  - 바나나
- 유제품
  - 우유
  - 치즈

## 기타 요소 — abbr, sub, sup, kbd, mark

### 구문

```markdown
<abbr title="Graphics Interchange Format">GIF</abbr>는 비트맵 이미지 형식입니다.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

세션을 종료하려면 <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd>를 누르세요.

대부분의 <mark>도롱뇽</mark>은 야행성이며, 곤충, 벌레 및 기타 작은 생물을 사냥합니다.
```

### 출력

<abbr title="Graphics Interchange Format">GIF</abbr>는 비트맵 이미지 형식입니다.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

세션을 종료하려면 <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd>를 누르세요.

대부분의 <mark>도롱뇽</mark>은 야행성이며, 곤충, 벌레 및 기타 작은 생물을 사냥합니다.
