### [원문 : 마크다운 가이드 홈페이지](https://www.markdownguide.org/extended-syntax/).

# Extended Syntax

**Advanced features that build on the basic Markdown syntax.**

**기본 Markdown 구문을 기반으로하는 고급 기능.**

## Overview

The basic syntax outlined in John Gruber’s original design document added many of the elements needed on a day-to-day basis, but it wasn’t enough for some people.

John Gruber의 설계 문서에 요약 된 기본 구문엔 많은 요소가 있음에도 일부 사람들에게는 충분하지 않았습니다.

That’s where extended syntax comes in.

이로인해 확장된 구문이 나오게 되었습니다.

Several individuals and organizations took it upon themselves to extend the basic syntax by adding additional elements like tables, code blocks, syntax highlighting, URL auto-linking, and footnotes.

여러 개인과 조직은 테이블, 코드 블록, 구문 강조, URL 자동 링크 및 각주와 같은 추가 요소를 추가하여 기본 구문을 직접 확장하여 사용하기 시작했습니다.

These elements can be enabled by using a lightweight markup language that builds upon the basic Markdown syntax, or by adding an extension to a compatible Markdown processor.

이러한 요소는 기본 마크 다운 구문을 기반으로하는 경량 마크 업 언어를 사용하거나 호환 가능한 마크 다운 프로세서에 확장을 추가하여 활성화 할 수 있습니다.

## Availability

Not all Markdown applications support extended syntax elements.

모든 Markdown 응용 프로그램이 확장 구문 요소를 지원하는 것은 아닙니다.

You’ll need to check whether or not the lightweight markup language your application is using supports the extended syntax elements you want to use.

응용 프로그램에서 사용하는 경량 마크 업 언어가 사용하려는 확장 구문 요소를 지원하는지 확인해야합니다.

If it doesn’t, it may still be possible to enable extensions in your Markdown processor.

그렇지 않은 경우 여전히 마크 다운 프로세서에서 확장 프로그램을 사용하도록 설정하는 것이 가능할 수 있습니다.

## Lightweight Markup Languages

There are several lightweight markup languages that are supersets of Markdown.

Markdown의 상위 집합 인 몇 가지 간단한 마크 업 언어가 있습니다.

They include Gruber’s basic syntax and build upon it by adding additional elements like tables, code blocks, syntax highlighting, URL auto-linking, and footnotes.

여기에는 Gruber의 기본 구문이 포함되며 테이블, 코드 블록, 구문 강조, URL 자동 링크 및 각주와 같은 추가 요소가 추가되어있습니다.

Many of the most popular Markdown applications use one of the following lightweight markup languages:

가장 많이 사용되는 Markdown 응용 프로그램은 다음과 같은 간단한 마크 업 언어 중 하나를 사용합니다.

- [CommonMark](https://commonmark.org/)
- [GitHub Flavored Markdown (GFM)](https://github.github.com/gfm/)
- [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/)
- [MultiMarkdown](https://fletcherpenney.net/multimarkdown/)
- [R Markdown](https://rmarkdown.rstudio.com/)

## Markdown Processors

There are [dozens of Markdown processors](https://github.com/markdown/markdown.github.com/wiki/Implementations) available.

사용 가능한 [마크 다운 프로세서](https://github.com/markdown/markdown.github.com/wiki/Implementations)는 수십 가지가 있습니다.

Many of them allow you to add extensions that enable extended syntax elements.

이것들은 대부분 확장구문을 지원합니다.

Check your processor’s documentation for more information.

더많은 정보는 프로세서의 문서를 확인하세요

## Tables

To add a table, use three or more hyphens (---) to create each column’s header,and use pipes (|) to separate each column.

표를 추가하려면 세 개 이상의 하이픈 (---)을 사용하여 각 열의 머리글을 만들고 파이프 (|)를 사용하여 각 열을 구분하십시오

You can optionally add pipes on either end of the table.

선택적으로 테이블의 양쪽 끝에 파이프를 추가 할 수 있습니다.

```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

Cell widths can vary, as shown below. The rendered output will look the same.

셀 너비는 아래와 같이 달라질 수 있습니다. 렌더링 된 출력은 동일하게 보입니다.

```
| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |
```

> Tip: Creating tables with hyphens and pipes can be tedious. To speed up the process, try using the [Markdown Tables Generator](http://www.tablesgenerator.com/markdown_tables). Build a table using the graphical interface, and then copy the generated Markdown-formatted text into your file.


> 팁 : 하이픈과 파이프가있는 테이블을 만드는 것은 번거로울 수 있습니다. 프로세스 속도를 높이려면 [Markdown Tables Generator](http://www.tablesgenerator.com/markdown_tables)를 사용해보십시오. 그래픽 인터페이스를 사용하여 테이블을 작성한 다음 생성 된 마크 다운 형식 텍스트를 파일에 복사하십시오.


## Alignment

You can align text in the columns to the left, right, or center by adding a colon (:) to the left, right, or on both side of the hyphens within the header row.

머리글 행의 왼쪽, 오른쪽 또는 하이픈 양쪽에 콜론 (:)을 추가하여 열의 텍스트를 왼쪽, 오른쪽 또는 가운데 정렬 할 수 있습니다.

```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

| Syntax    | Description |   Test Text |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here's this |
| Paragraph |    Text     |    And more |

## Formatting Text in Tables

You can format the text within tables.

표 내에서 텍스트 서식을 지정할 수 있습니다

For example, you can add links, code (words or phrases in backticks (`) only, not code blocks), and emphasis.

예를 들어, 링크, 코드 (코드 블록이 아닌 역따옴표(`)의 단어 또는 구만) 및 강조를 추가 할 수 있습니다.

You can’t add headings, blockquotes, lists, horizontal rules, images, or HTML tags.

제목, 블록 인용 부호, 목록, 가로 규칙, 이미지 또는 HTML 태그는 추가 할 수 없습니다.

## Escaping Pipe Characters in Tables

You can display a pipe (|) character in a table by using its HTML character code (&#124;).

HTML 문자 코드 (\&#124;)를 사용하여 테이블에 파이프 (|) 문자를 표시 할 수 있습니다.

## Fenced Code Blocks

The basic Markdown syntax allows you to create code blocks by indenting lines by four spaces or one tab.

기본 마크 다운 구문을 사용하면 네 개의 공백이나 하나의 탭으로 줄을 들여 쓰기하여 코드 블록을 만들 수 있습니다.

If you find that inconvenient, try using fenced code blocks.

그 방법이 불편하다면, 중괄호를 이용하세요

Depending on your Markdown processor or editor, you’ll use three backticks (```) or three tildes (~~~) on the lines before and after the code block.

마크 다운 프로세서 또는 편집기에 따라 코드 블록 앞뒤의 줄에 3 개의 역따옴표(```) 또는 3 개의 물결표 (~~~)를 사용합니다.

The best part? You don’t have to indent any lines!

가장 좋은점은 들여쓰기를 할 필요가 없다는 것입니다!

```

```

{
"firstName": "John",
"lastName": "Smith",
"age": 25
}

```

```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

> Tip: Need to display backticks inside a code block? See this [section](./BasicSyntax.md#escaping-backticks) to learn how to escape them.

> 팁 : 코드 블록 안에 역따옴표를 표시해야합니까? 역따옴표 [이스케이핑](./BasicSyntax.md#escaping-backticks) 하기

## Syntax Highlighting

Many Markdown processors support syntax highlighting for fenced code blocks.

많은 Markdown 프로세서는 중괄호 코드 블록에 대한 구문 강조를 지원합니다

This feature allows you to add color highlighting for whatever language your code was written in.

이 기능을 사용하면 코드가 작성된 언어에 대한 색상 강조 표시를 추가 할 수 있습니다.

To add syntax highlighting, specify a language next to the backticks before the fenced code block.

구문 강조를 추가하려면 분리 코드 블록 앞에 역따옴표 옆에 언어를 지정하십시오.

````
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
````

````

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
````

## Footnotes (깃허브는 지원하지 않습니다.)

Footnotes allow you to add notes and references without cluttering the body of the document.

각주를 사용하면 문서 본문을 어지럽히 지 않고도 메모 및 참조를 추가 할 수 있습니다.

When you create a footnote, a superscript number with a link appears where you added the footnote reference.

각주를 만들면 각주 참조를 추가 한 위치에 링크가있는 위첨자 번호가 나타납니다.

Readers can click the link to jump to the content of the footnote at the bottom of the page.

독자는 링크를 클릭하며, 페이지 아래쪽의 각주내용으로 이동할 수 있습니다.

To create a footnote reference, add a caret and an identifier inside brackets ([^1]).

각주 참조를 만들려면 대괄호 안에 캐럿과 식별자를 추가하십시오 ([^ 1]).

Identifiers can be numbers or words, but they can’t contain spaces or tabs.

식별자는 숫자 나 단어 일 수 있지만 공백이나 탭을 포함 할 수 없습니다.

Identifiers only correlate the footnote reference with the footnote itself — in the output, footnotes are numbered sequentially.

식별자는 각주 참조를 각주 자체와 만 관련시킵니다. 출력에서 각주는 번호가 순차적으로 매겨집니다.

Add the footnote using another caret and number inside brackets with a colon and text ([^1]: My footnote.).

콜론과 텍스트 ([^ 1] : My footnote.)와 함께 대괄호 안에 다른 캐럿과 숫자를 사용하여 각주를 추가하십시오.

You don’t have to put footnotes at the end of the document.

각주를 문서 끝에 놓을 필요는 없습니다.

You can put them anywhere except inside other elements like lists, block quotes, and tables.

목록, 블록 따옴표 및 테이블과 같은 다른 요소 내부를 제외하고 어디에나 넣을 수 있습니다.

```
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.
[^bignote]: Here's one with multiple paragraphs and code.

  Indent paragraphs to include them in the footnote.

  `{ my code }`

  Add as many paragraphs as you like.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

Here's a simple footnote,<sup>[1]</sup> and here's a longer one.↩

1. This is the first footnote.↩
2. Here's one with multiple paragraphs and code.

      Indent paragraphs to include them in the footnote.

      `{ my code }`

      Add as many paragraphs as you like.↩

## Heading IDs

Many Markdown processors support custom IDs for [headings](./BasicSyntax.md#headings) — some Markdown processors automatically add them.

많은 Markdown 프로세서는 [제목](./BasicSyntax.md#headings)에 대한 사용자 정의 ID를 지원합니다. 일부 Markdown 프로세서는 자동으로 추가합니다

Adding custom IDs allows you to link directly to headings and modify them with CSS.

사용자 정의 ID를 추가하면 제목에 직접 연결하여 CSS로 수정할 수 있습니다.

To add a custom heading ID, enclose the custom ID in curly braces on the same line as the heading.

맞춤 제목 ID를 추가하려면 맞춤 ID를 제목과 같은 줄에 중괄호로 묶습니다.

```
### My Great Heading {#custom-id}
```

The HTML looks like this:

렌더링 결과 는 다음과 같습니다.

```
<h3 id="custom-id">My Great Heading</h3>
```

## Linking to Heading IDs

You can link to headings with custom IDs in the file by creating a standard link with a number sign (#) followed by the custom heading ID.

숫자 기호 (#)와 사용자 정의 표제 ID가있는 표준 링크를 작성하여 파일에서 사용자 정의 ID로 표제에 링크 할 수 있습니다.

| Markdown                     | HTML                                     | Rendered Output             |
| ---------------------------- | ---------------------------------------- | --------------------------- |
| \[Heading IDs](#heading-ids) | \<a href="#heading-ids">Heading IDs\</a> | [Heading IDs](#heading-ids) |

Other websites can link to the heading by adding the custom heading ID to the full URL of the webpage (e.g, [Heading IDs](https://www.markdownguide.org/extended-syntax#heading-ids)).

다른 웹 사이트는 웹 페이지의 전체 URL에 맞춤 제목 ID를 추가하여 제목에 연결할 수 있습니다 (예 : [제목 ID](https://www.markdownguide.org/extended-syntax#heading-ids)).

## Definition Lists

Some Markdown processors allow you to create definition lists of terms and their corresponding definitions.

일부 마크 다운 프로세서를 사용하면 용어 정의 목록과 해당 정의를 만들 수 있습니다.

To create a definition list, type the term on the first line.

정의 목록을 작성하려면 첫 번째 행에 용어를 입력하십시오.

On the next line, type a colon followed by a space and the definition.

다음 줄에 콜론과 공백 및 정의를 입력하십시오.

```
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```

The HTML looks like this:

HTML 은 다음과 같습니다.

```
<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term. </dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

## Strikethrough

You can “strikethrough” words by putting a horizontal line through the center of them. The result looks ~~like this~~.

단어 가운데에 가로 선을 넣어 "취소선" 을 입력 할 수 있습니다. 결과는 ~~다음과 같습니다~~

This feature allows you to indicate that certain words are a mistake not meant for inclusion in the document.

이 기능을 사용하면 특정 단어가 문서에 포함되지 않은 실수임을 나타낼 수 있습니다

To strikethrough words, use two tilde symbols (~~) before and after the words.

취소선을 넣으려면, 단어 앞뒤에 두 개의 물결 기호 (~~)를 사용하십시오.

```
~~The world is flat.~~ We now know that the world is round.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

~~The world is flat.~~ We now know that the world is round.

## Task Lists

Task lists allow you to create a list of items with checkboxes.

작업 목록을 사용하면 체크박스가 있는 항목 목록을 만들 수 있습니다.

In Markdown applications that support task lists, checkboxes will be displayed next to the content.

작업 목록을 지원하는 마크 다운 응용 프로그램에서 내용 옆에 체크박스가 표시됩니다.

To create a task list, add dashes (-) and brackets with a space ([ ]) in front of task list items.

목록을 만들려면 작업 목록 항목 앞에 공백 ([])이있는 대시 (-) 및 괄호를 추가하십시오.

To select a checkbox, add an x in between the brackets ([x]).

체크박스를 선택하려면 괄호 ([x]) 사이에 x를 추가하십시오.

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

## Automatic URL Linking

Many Markdown processors automatically turn URLs into links.

많은 마크 다운 프로세서가 자동으로 URL을 링크로 바꿉니다.

That means if you type http://www.example.com, your Markdown processor will automatically turn it into a link even though you haven’t used brackets.

즉, http://www.example.com을 입력하면 마크 다운 프로세서는 대괄호를 사용하지 않아도 자동으로 링크로 전환됩니다.

```
http://www.example.com
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

http://www.example.com

## Disabling Automatic URL Linking

If you don’t want a URL to be automatically linked, you can remove the link by denoting the URL as code with backticks.

URL이 자동으로 연결되지 않게하려면 URL을 역따옴표가 있는 코드로 표시하여 링크를 제거 할 수 있습니다.

```
`http://www.example.com`
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

`http://www.example.com`
