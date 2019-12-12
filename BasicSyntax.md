# Basic Syntax

**The Markdown elements outlined in John Gruber's design document.**

**John Gruber의 설계 문서에 설명 된 Markdown 요소**

## Overview

Nearly all Markdown applications support the basic syntax outlined in John Gruber’s original design document.

거의 대부분의 Markdown 어플리케이션은 John Gruber 의 원본 설계 문서에 기반한 기본 구문을 지원합니다.

There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible.

Markdown 프로세서 간에는 약간의 변형 및 불일치가 있으며, 가능한경우 인라인으로 표시됩니다

> Note: Using Markdown doesn't mean that you can't also use HTML. You can add HTML tags to any Markdown file. This is helpful if you prefer certain HTML tags to Markdown syntax. For example, some people find that it's easier to use HTML tags for images.

> 참고 : Mardown 을 사용한다는것이 HTML 을 사용하지 못한다는 의미는 아닙니다. 어떤 Markdown 파일에도 HTML을 사용할 수 있습니다. 마크 다운 구문보다 특정 HTML 태그를 선호하는 경우에 유용합니다. 예를들면, 어떤사람들은 이미지에 HTML 태그를 사용하는것이 더 쉽다고 할 수 도 있습니다.

## Headings

To create a heading, add number signs (#) in front of a word or phrase.

heading 을 만들기위해서, 단어나 문장 앞에 해시태그(#) 를 추가 하세요.

The number of number signs you use should correspond to the heading level.

해시태그의 갯수가 heading 레벨에 해당합니다.

For example, to create a heading level three (\<h3>), use three number signs (e.g., ### My Header).

예를들어, heading 레벨 3 (\<h3>) 을 표기하려면, 해시태그를 3개 사용하세요 ( 예) \#\#\# My Header )

| Markdown                     | HTML                       | Rendered Output   |
| ---------------------------- | -------------------------- | ----------------- |
| \# Heading level 1           | \<h1>Heading level 1\</h1> | # Heading level 1 |
| \#\# Heading level 2         | \<h2>Heading level 2\</h2> | # Heading level 2 |
| \#\#\# Heading level 3       | \<h3>Heading level 3\</h3> | # Heading level 3 |
| \#\#\#\# Heading level 4     | \<h4>Heading level 4\</h4> | # Heading level 4 |
| \#\#\#\#\# Heading level 5   | \<h5>Heading level 5\</h5> | # Heading level 5 |
| \#\#\#\#\#\# Heading level 6 | \<h6>Heading level 6\</h6> | # Heading level 6 |

## Alternate Syntax

Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

또는, 제목수준 1의 텍스트 아래 쪽에 == 를 추가하거나, 제목수준 2의 텍스트 아래쪽에 -- 를 추가 하는 방법도 있습니다.

| Markdown                            | HTML                       | Rendered Output   |
| ----------------------------------- | -------------------------- | ----------------- |
| Heading level 1<br>\=============== | \<h1>Heading level 1\</h1> | # Heading level 1 |
| Heading level 2<br>\--------------- | \<h2>Heading level 2\</h2> | # Heading level 2 |

## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

단락을 만들려면 빈 줄을 사용하여 하나 이상의 텍스트 줄을 구분하십시오.

You should not indent paragraphs with spaces or tabs.

공백이나 탭이있는 단락을 들여 쓰면 안됩니다.

| Markdown                                                                                            | HTML                                                                                                                  | Rendered Output                                                                                     |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on. | \<p>I really like using Markdown.\</p><br><br>\<p>I think I'll use it to format all of my documents from now on.\</p> | I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on. |

## Line Breaks

To create a line break (\<br>), end a line with two or more spaces, and then type return.

줄 바꿈 (\<br>)을 만들려면 두 개 이상의 공백으로 줄을 끝내고 return을 입력하십시오.(번역자는 이거 잘 안되었음...;;)

| Markdown                                             | HTML                                                               | Rendered Output                                          |
| ---------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------- |
| This is the first line. And this is the second line. | \<p>This is the first line.\<br> And this is the second line.\</p> | This is the first line.<br> And this is the second line. |

## Emphasis

You can add emphasis by making text bold or italic.

텍스트를 굵게 또는 이탤릭체로 강조할 수 있습니다.

### Bold

To bold text, add two asterisks or underscores before and after a word or phrase.

글자 앞뒤에 별표나 언더스코어를 추가하여 글자를 굵게 할 수 있습니다.

To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

단어 중간의 글자를 굵게 하려면, 공백없이 단어 앞뒤에 별표를 추가하세요

| Markdown                       | HTML                                      | Rendered Output                         |
| ------------------------------ | ----------------------------------------- | --------------------------------------- |
| I just love \*\*bold text\*\*. | I just love \<strong>bold text\</strong>. | I just love <strong>bold text</strong>. |
| I just love \*\*bold text\*\*. | I just love \<strong>bold text\</strong>. | I just love <strong>bold text</strong>. |
| Love\*\*is\*\*bold             | Love\<strong>is\</strong>bold             | Love<strong>is</strong>bold             |

### Italic

To italicize text, add one asterisk or underscore before and after a word or phrase.

별 하나 또는 언더스코어 하나를 글자 앞뒤에 추가하여, 이탤릭체로 표시할 수 있습니다.

To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

단어 중간의 글자를 이탤릭체로 표시하려면, 공백없이 단어 앞뒤에 별표를 추가하세요

| Markdown          | HTML                       | Rendered Output          |
| ----------------- | -------------------------- | ------------------------ |
| the _cat's meow_. | the \<em>cat's meow\</em>. | the <em>cat's meow</em>. |
| the _cat's meow_. | the \<em>cat's meow\</em>. | the <em>cat's meow</em>. |
| A\*cat\*meow      | A\<em>cat\</em>meow        | A<em>cat</em>meow        |

### Bold and Italic

To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase.

글자를 굵은 이탤릭체로 표기하기위해, 별표와 언더스코어를 함께 사용 할 수 도 있습니다.

| Markdown                       | HTML                                            | Rendered Output                    |
| ------------------------------ | ----------------------------------------------- | ---------------------------------- |
| This is \*\*\*very nice\*\*\*. | This is \<strong>\<em>very nice\</em>\</strong> | This is <strong><em>very nice</em> |
| This is \_\_\_very nice\_\_\_. | This is \<strong>\<em>very nice\</em>\</strong> | This is <strong><em>very nice</em> |
| This is \*\*\_very nice\_\*\*. | This is \<strong>\<em>very nice\</em>\</strong> | This is <strong><em>very nice</em> |
| This is \_\_\*very nice\*\_\_. | This is \<strong>\<em>very nice\</em>\</strong> | This is <strong><em>very nice</em> |

## Blockquotes

To create a blockquote, add a > in front of a paragraph.

인용구를 만들려면 단락 앞에 > 를 추가하십시오.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

> Dorothy followed her through many of the beautiful rooms in her castle.

### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

인용 부호는 여러 단락을 포함 할 수 있습니다. 단락 사이의 빈 줄에 > 를 추가하십시오.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### Nested Blockquotes

Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

인용 부호는 중첩 될 수 있습니다. 중첩하려는 단락 앞에 >>를 추가하십시오.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### Blockquotes with Other Elements

Blockquotes can contain other Markdown formatted elements.

인용구에는 다른 마크 다운 형식 요소가 포함될 수 있습니다.

Not all elements can be used — you’ll need to experiment to see which ones work.

모든 요소를 ​​사용할 수있는 것은 아닙니다. 어떤 요소가 효과가 있는지 실험 해 봐야합니다.

```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>   _Everything_ is going according to **plan**.
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>   _Everything_ is going according to **plan**.

## Lists

You can organize items into ordered and unordered lists.

항목을 정렬 된 목록과 정렬되지 않은 목록으로 구성 할 수 있습니다.

### Ordered Lists

To create an ordered list, add line items with numbers followed by periods.

정렬된 목록을 만드려면, 순서를 표기하여 항목을 나열하세요

The numbers don’t have to be in numerical order, but the list should start with the number one.

목록 순서의 숫자는 섞여도 되지만, 1부터 시작하세요

<table>
  <thead>
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>Rendered Output</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td>
        1. First item<br>
        2. Second item<br>
        3. Third item<br>
        4. Fourth item
    </td>
    <td>
        &lt;ol&gt;<br>
          &lt;li&gt;First item&lt;/li&gt;<br>
          &lt;li&gt;Second item&lt;/li&gt;<br>
          &lt;li&gt;Third item&lt;/li&gt;<br>
          &lt;li&gt;Fourth item&lt;/li&gt;<br>
        &lt;/ol&gt;
    </td>
    <td>
      <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
        <li>Fourth item</li>
      </ol>
    </td>
    </tr>
    <tr>
      <td>
          1. First item<br>
          1. Second item<br>
          1. Third item<br>
          1. Fourth item
      </td>
      <td>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
          1. First item<br>
          8. Second item<br>
          3. Third item<br>
          5. Fourth item
      </td>
      <td>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
          1. First item<br>
          2. Second item<br>
          3. Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;1. Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;2. Indented item<br>
          1. Fourth item
      </td>
      <td>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item<br>
              &lt;ol&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
              &lt;/ol&gt;<br>
            &lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item
            <ol>
              <li>Indented item</li>
              <li>Indented item</li>
            </ol>
          </li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

### Unordered Lists

To create an unordered list, add dashes (-), asterisks (\*), or plus signs (+) in front of line items.

순서가없는 목록을 만들려면 항목 앞에 대시 (-), 별표 (\*) 또는 더하기 기호 (+)를 추가하십시오.

Indent one or more items to create a nested list.

중첩 된 목록을 만들려면 하나 이상의 항목을 들여 씁니다.

<table>
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>Rendered Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
          - First item<br>
          - Second item<br>
          - Third item<br>
          - Fourth item
      </td>
      <td>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
          * First item<br>
          * Second item<br>
          * Third item<br>
          * Fourth item
      </td>
      <td>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
          + First item<br>
          * Second item<br>
          - Third item<br>
          + Fourth item
      </td>
      <td>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
          - First item<br>
          - Second item<br>
          - Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          - Fourth item
      </td>
      <td>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item<br>
              &lt;ul&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
              &lt;/ul&gt;<br>
            &lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item
            <ul>
              <li>Indented item</li>
              <li>Indented item</li>
            </ul>
          </li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

목록의 연속성을 유지하면서 목록에 다른 요소를 추가하려면 다음 예와 같이 요소를 4 칸 또는 탭으로 들여 쓰기하십시오.

#### Paragraphs

```
- This is the first list item.
- Here's the second list item.

  I need to add another paragraph below the second list item.

- And here's the third list item.
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

- This is the first list item.
- Here's the second list item.

  I need to add another paragraph below the second list item.

- And here's the third list item.

#### Blockquotes

```
- This is the first list item.
- Here's the second list item.

  > A blockquote would look great below the second list item.

- And here's the third list item.
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

- This is the first list item.
- Here's the second list item.

  > A blockquote would look great below the second list item.

- And here's the third list item

#### Code Blocks

Code blocks are normally indented four spaces or one tab.

코드 블록은 일반적으로 4 개의 공백 또는 1 개의 탭으로 들여 쓰기됩니다.

When they’re in a list, indent them eight spaces or two tabs.

목록에있을 때 여백 8 개 또는 탭 2 개를 들여 씁니다.

```
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

#### Images

```
1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](https://cdn.pixabay.com/photo/2012/04/26/19/47/penguin-42936_960_720.png)

3.  Close the file.
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](https://cdn.pixabay.com/photo/2012/04/26/19/47/penguin-42936_960_720.png)

3.  Close the file.

## Code

To denote a word or phrase as code, enclose it in backticks (`).

단어 나 문구를 코드로 나타내려면 역따옴표(`)로 묶습니다.

| Markdown                              | HTML                                             | Rendered Output                     |
| ------------------------------------- | ------------------------------------------------ | ----------------------------------- |
| At the command prompt, type \`nano\`. | At the command prompt, type \<code>nano\</code>. | At the command prompt, type `nano`. |

### Escaping Backticks

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (``).

코드로 표시하려는 단어 나 구에 하나 이상의 백틱이 포함 된 경우 단어 나 구를 이중 역따옴표(``)으로 묶어 이스케이프 처리 할 수 ​​있습니다.

| Markdown                                      | HTML                                               | Rendered Output                         |
| --------------------------------------------- | -------------------------------------------------- | --------------------------------------- |
| \`\` Use \`code\` in your Markdown file. \`\` | \<code>Use \`code\` in your Markdown file.\</code> | `` Use `code` in your Markdown file. `` |

### Code Blocks

To create code blocks, indent every line of the block by at least four spaces or one tab.

코드 블록을 만들려면 블록의 모든 줄을 최소 4 개의 공백이나 하나의 탭으로 들여 씁니다.

```
    <html>
      <head>
      </head>
    </html>
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

    <html>
      <head>
      </head>
    </html>

```
Note: To create code blocks without indenting lines, use fenced code blocks.
```

```
참고 : 들여 쓰기 줄없이 코드 블록을 만들려면 중괄호 코드 블록을 사용하십시오.
```

## Horizontal Rules

To create a horizontal rule, use three or more asterisks (\*\*\*), dashes (---), or underscores (\_\_\_) on a line by themselves.

구분선을 추가 하려면 별표 (\*\*\*), 대시 (---) 또는 밑줄 (\_\_\_)을 세 개 이상 사용하십시오.

```
***

---

___

```

The rendered output of all three looks identical:

세가지 렌더링 결과는 다음과 같이 동일하게 나타납니다.

---

## Links

To create a link, enclose the link text in brackets (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., (https://duckduckgo.com)).

링크를 만들기위해, 대괄호 안에 문구를 입력하고 바로뒤의 소괄호에 링크경로를 입력해주세요

'''
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
'''

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

### Adding Titles

You can optionally add a title for a link.

옵션으로 링크에 타이틀을 추가 할 수 있습니다.

This will appear as a tooltip when the user hovers over the link.

이 경우 링크에 마우스를 올리면 툴팁이 나타나게 됩니다.

To add a title, enclose it in parentheses after the URL.

타이틀을 추가하기 위해선, 경로 뒤에 문구를 추가 하세요

```
My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").

### URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

URL 또는 이메일주소를 즉석하여 링크로 바꾸려면 꺽쇠로 묶어주세요

```
<https://www.markdownguide.org>
<fake@example.com>
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

<https://www.markdownguide.org>
<fake@example.com>

### Formatting Links

To emphasize links, add asterisks before and after the brackets and parentheses.

링크를 강조하기위해선 대괄호 앞뒤에 별표를 추가 하세요

To denote links as code, add backticks in the brackets.

링크를 코드로 표시하기위해서는 대괄호 안에 역따옴표를 추가하세요

```
I love supporting the **[EFF](https://eff.org)**.
This is the _[Markdown Guide](https://www.markdownguide.org)_.
See the section on [`code`](#code).
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

I love supporting the **[EFF](https://eff.org)**.
This is the _[Markdown Guide](https://www.markdownguide.org)_.
See the section on [`code`](#code).

### Reference-style Links

Reference-style links are a special kind of link that make URLs easier to display and read in Markdown.

참조 스타일 링크는 마크 다운에서 URL을보다 쉽게 ​​표시하고 읽을 수 있도록하는 특수한 종류의 링크입니다.

Reference-style links are constructed in two parts: the part you keep inline with your text and the part you store somewhere else in the file to keep the text easy to read.

참조 스타일 링크는 두 부분으로 구성됩니다. 텍스트와 인라인으로 유지하는 부분과 텍스트를 쉽게 읽을 수 있도록 파일의 다른 곳에 저장 한 부분입니다.

#### Formatting the First Part of the Link

The first part of a reference-style link is formatted with two sets of brackets.

참조 스타일 링크의 첫 번째 부분은 두 개의 대괄호로 구성됩니다.

The first set of brackets surrounds the text that should appear linked.

첫 번째 대괄호 세트는 링크 된 텍스트를 둘러 쌉니다.

The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

두 번째 대괄호 세트는 문서의 다른 곳에 저장하는 링크를 가리키는 데 사용되는 레이블을 표시합니다.

Although not required, you can include a space between the first and second set of brackets.

필수는 아니지만 첫 번째와 두 번째 대괄호 사이에 공백을 포함 할 수 있습니다.

The label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

두 번째 대괄호 세트의 레이블은 대소 문자를 구분하지 않으며 문자, 숫자, 공백 또는 문장 부호를 포함 할 수 있습니다.

This means the following example formats are roughly equivalent for the first part of the link:

이는 다음 예제는 링크의 첫 번째 부분과 거의 동일 함을 의미합니다.

- [hobbit-hole][1]
- [hobbit-hole][1]

#### Formatting the Second Part of the Link

The second part of a reference-style link is formatted with the following attributes:

참조 스타일 링크의 두 번째 부분은 다음 속성으로 형식화됩니다.

1. The label, in brackets, followed immediately by a colon and at least one space (e.g., [label]: ).
2. The URL for the link, which you can optionally enclose in angle brackets.
3. The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

4. 대괄호로 묶인 레이블 뒤에 바로 콜론과 하나 이상의 공백이옵니다. (예) [label]: ).
5. 꺽쇠괄호는 옵션입니다.
6. 링크 제목은 소괄호, 홑따옴표, 쌍따옴표로 묶을 수 도 있습니다.

This means the following example formats are all roughly equivalent for the second part of the link:

- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
- \[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
- \[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
- \[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)

You can place this second part of the link anywhere in your Markdown document.

이 두번째 부분은 마크다운 문서 어디에나 둘 수 있습니다.

Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document (like endnotes or footnotes).

사람에 따라, 이 부분을 문단 바로 뒤에 배치하거나 문서의 마지막에 배치하곤 합니다. (미주나 각주와 같이)

#### An Example Putting the Parts Together

Say you add a URL as a standard URL link to a paragraph and it looks like this in Markdown:

마크다운에 다음과 같이 URL을 삽입했다고 가정합니다.

```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
```

Though it may point to interesting additional information, the URL as displayed really doesn’t add much to the existing raw text other than making it harder to read.

흥미로운 추가 정보를 지적 할 수도 있지만, 표시되는 URL은 실제로 읽기가 더 어려워 질뿐 아니라 기존의 원본 텍스트에 추가되지 않습니다.

To fix that, you could format the URL like this instead:

다음과 같은 포맷으로 수정할 수 있습니다.

```
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.

[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
```

In both instances above, the rendered output would be identical:

위의 두 경우 모두 렌더링 결과는 동일합니다.

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.

and the HTML for the link would be:

링크의 HTML 포맷은 다음과 같습니다.

```
<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>
```

## Images

To add an image, add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses.

이미지를 추가하기위해선 느낌표를 이용하세요. 느낌표 뒤에 대괄호로 이미지의 대체문구 를 기입하고, 이어서 소괄호로 이미지의 경로를 입력하세요.

You can optionally add a title after the URL in the parentheses.

이미지 경로 뒤에 이미지 타이틀을 선택적으로 입력 가능합니다.

```
![아지아지 하얀강아지](https://cdn.pixabay.com/photo/2019/12/06/17/44/japanese-4677848_1280.jpg "흰 개")
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

![아지아지 하얀강아지](https://cdn.pixabay.com/photo/2019/12/06/17/44/japanese-4677848_1280.jpg "흰 개")

### Linking Images

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

이미지에 링크를 추가하려면 이미지의 마크 다운을 대괄호로 묶은 다음, 구문 뒤에 링크를 소괄호로 묶어 연결하세요

```
[![로맨틱한 벨기에](https://cdn.pixabay.com/photo/2019/11/29/14/18/gent-4661419_1280.jpg "운하 옆으로 로맨틱 한 불빛에 빛나는 건물들")](https://pixabay.com/ko/photos/%EC%8B%A0%EC%82%AC-%EB%AF%B8%EB%9F%AC%EB%A7%81-%EB%AC%BC-%EB%B6%84%EC%A7%80-%EB%B2%A8%EA%B8%B0%EC%97%90-4661419/)
```

The rendered output looks like this:

렌더링 결과 는 다음과 같습니다.

[![로맨틱한 벨기에](https://cdn.pixabay.com/photo/2019/11/29/14/18/gent-4661419_1280.jpg "운하 옆으로 로맨틱 한 불빛에 빛나는 건물들")](https://pixabay.com/ko/photos/%EC%8B%A0%EC%82%AC-%EB%AF%B8%EB%9F%AC%EB%A7%81-%EB%AC%BC-%EB%B6%84%EC%A7%80-%EB%B2%A8%EA%B8%B0%EC%97%90-4661419/)

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (\) in front of the character.

마크 다운 문서에서 텍스트 서식을 지정하는 데 사용되는 리터럴 문자를 표시하려면 문자 앞에 백 슬래시 (\)를 추가하십시오

```
\* Without the backslash, this would be a bullet in an unordered list.
```

```
\* 백슬래쉬가 없으면, 순서 없는 목록의 점 기호로 보이게 됩니다.
```

The rendered output looks like this:

다음과 같이 렌더링 됩니다.

- Without the backslash, this would be a bullet in an unordered list.

- 백슬래쉬가 없으면, 순서 없는 목록의 점 기호로 보이게 됩니다.

### Characters You Can Escape

You can use a backslash to escape the following characters.

백슬래쉬를 이용하여 다음 문자들은 이스케이프 가능 합니다.

| Character                                          | Name                                    |
| -------------------------------------------------- | --------------------------------------- |
| \\                                                 | backslash                               |
| ` | backtick (see also escaping backticks in code) |
| \*                                                 | asterisk                                |
| \_                                                 | underscore                              |
| { }                                                | curly braces                            |
| [ ]                                                | brackets                                |
| ( )                                                | parentheses                             |
| #                                                  | pound sign                              |
| +                                                  | plus sign                               |
| -                                                  | minus sign (hyphen)                     |
| .                                                  | dot                                     |
| !                                                  | exclamation mark                        |
| \|                                                 | pipe (see also escaping pipe in tables) |
