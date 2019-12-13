### [원문 : 마크다운 가이드 홈페이지](https://www.markdownguide.org/).

# Markdown Cheat Sheet
**A quick reference to the Markdown syntax.**

**마크다운 구문 빠른 참고**

## Overview
This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. 

Markdown cheat sheet 는 모든 마크 다운 구문 요소에 대한 간략한 개요를 제공합니다.

It can’t cover every edge case, so if you need more information about any of these elements, refer to our reference guides for basic syntax and extended syntax.

모든 경우의 수를 다룰 수 없으므로, 더 많은 정보가 필요한 경우, 기본구문(basic syntax)과 확장구문(extended syntax)을 참조하십시오.

## Basic Syntax
These are the elements outlined in John Gruber’s original design document.

이 요소들은 John Gruber가 작성한 기본 설계 문서의 개요 입니다. 

All Markdown applications support these elements.

모든 Markdown 애플리케이션은 이러한 요소를 지원합니다.

| Element	| Markdown Syntax | 
| ----------- | ----------- |
| [Heading](./BasicSyntax.md#headings) | # H1 <br>## H2<br>### H3 |
| [Bold](./BasicSyntax.md#bold) | \*\*bold text\*\* |
| [Italic](./BasicSyntax.md#italic) | \*italicized text\* |
| [Blockquote](./BasicSyntax.md#blockquotes) | > blockquote |
| [Ordered List](./BasicSyntax.md#ordered-lists) | 1. First item <br>2. Second item <br>3. Third item |
| [Unordered List](./BasicSyntax.md#ordered-lists) | - First item <br>- Second item <br>- Third item |
| [Code](./BasicSyntax.md#code) | \`code\` |
| [Horizontal Rule](./BasicSyntax.md#horizontal-rules) | --- |
| [Link](./BasicSyntax.md#links) | \[title]\(https://www.example.com) |
| [Image](./BasicSyntax.md#images-1) | \![alt text]\(image.jpg) |

## Extended Syntax
These elements extend the basic syntax by adding additional features.

이 요소들은 추가 기능을 추가하여 기본 구문을 확장합니다.

Not all Markdown applications support these elements.

모든 Markdown 어플리케이션이 이 요소들을 지원하는것은 아닙니다. 

| Element	| Markdown Syntax |
| ----------- | ----------- |
| [Table](./ExtendedSyntax.md#tables) | \| Syntax \| Description \|<br>\| ----------- \| ----------- \|<br>\| Header \| Title \|<br>\| Paragraph \| Text \| |
| [Fenced Code Block](./ExtendedSyntax.md#fenced-code-blocks) | \```<br>{<br>  "firstName": "John",<br>  "lastName": "Smith",<br>  "age": 25<br>}<br>\``` |
| [Footnote](./ExtendedSyntax.md#footnotes) | Here's a sentence with a footnote. [^1]<br><br><br>[^1]: This is the footnote. |
| [Heading ID](./ExtendedSyntax.md#heading-ids) | ### My Great Heading \{#custom-id} |
| [Definition List](./ExtendedSyntax.md#definition-lists) | term <br>: definition |
| [Strikethrough](./ExtendedSyntax.md#strikethrough) | \~~The world is flat.~~ |
| [Task List](./ExtendedSyntax.md#task-lists) | - [x] Write the press release <br>- [ ] Update the website <br>- [ ] Contact the media |
