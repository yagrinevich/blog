---
title: Lightweight Markup Languages
date: 2022-04-08
math: true
image:
  location: 2
  caption: 'Image credit: [**John Moeses Bauan**](https://unsplash.com/photos/OGZtQF8iC0g)'
---

Lightweight Markup Languages: This is Why You Should Use AsciiDoc Instead of Regular Markdown


## What is a "markup language"?
 A markup language is a set of codes that, when applied to plain text, allows you to add one or more of the following properties (among others):

    Define Text
    Structure text
    Describe text layout
    Decorate text

One markup language that you come across every day (unless you're a hermit) is Hypertext Markup Language, or HTML. The websites and applications that bring you news and show you your email are built, at least in part, with HTML markup, using tags as a mechanism to mark up raw text content. For example, consider the following HTML snippet:
### Code




If you wanted to take advantage of markup languages, for example by publishing an HTML page on the web or converting a DocBook file to PDF so it can be printed, you had to do one of two things. On the one hand, you can spend time learning these languages ​​inside and out, writing them down by hand, and then triple-checking your work. Or you could invest in a tool that manages the difficulty for you.
Luckily, some enterprising developers have come up with a third option. They created new markup languages ​​that contained many (in some cases most or all) of the features of their heavier counterparts, but greatly simplified the syntax. These "light" languages ​​include the familiar Markdown as well as Asciidoc, the Egc format in Org mode, and the Mediawiki syntax.
### Story

###Story

Lightweight markup languages ​​were originally used on text displays that could not display italicized or bold characters, so informal methods had to be developed to communicate this information. This formatting choice has naturally been applied to plain text emails. Console browsers may also use similar rendering conventions.

In 1986, the international standard SGML provided a means to define and parse lightweight markup languages ​​using grammars and tag implication. 1998 W3C XML is an SGML profile that lacks these features. However, the SGML Document Type Definition (DTD) for any of the languages ​​listed below is not known.
### Types

Lightweight markup languages ​​can be categorized by their tag types. Similar to HTML (bold), some languages ​​use named elements that have a common format for start and end tags (e.g. BBCode [b] bold [/b]), while proper simplified markup languages ​​are limited to ASCII-only punctuation and others non-letter characters for tags, but some also mix both styles (eg Textile bq.) or allow inline HTML (eg Markdown ), possibly extended with custom elements (eg MediaWiki source).

Most languages ​​distinguish between markup for lines or blocks and shorter sections of text, but some only support inline markup.

Some markup languages ​​are designed for a specific purpose, such as documenting computer code (eg POD, RD ) or converting to a specific output format (usually HTML) and nothing else, others more generally in an application. This includes whether they are oriented towards text representation or data serialization.

Presentation oriented languages ​​include AsciiDoc, atx, BBCode, Creole, Crossmark, Epytext, Haml, JsonML, MakeDoc, Markdown, Org-mode, POD, reST, RD, Setext, SiSU, SPIP, Xupl, Texy!, Textile, txt2tags, UDO and Wikitext.

Data serialization-oriented languages ​​include Curl (homoicon but also reads JSON; each object is serialized), JSON, and YAML.
### Compare language features

The native Markdown syntax does not support class attributes or id attributes; however, since Markdown supports including native HTML, these features can be implemented using straight HTML. (Some extensions may support these features.)
The native txt2tags syntax does not support class attributes or id attributes; however, since txt2tags supports including native HTML code in tagged areas, these features can be implemented using straight HTML when stored in the target HTML.
### Simplified markup language syntax comparison
Хотя обычно документируется выделение текста курсивом и полужирным шрифтом, большинство облегченных процессоров разметки выводят семантические элементы HTML emи сильныйвместо этого. Моноширинный текст может привести либо к семантическому коду, либо к презентационным элементам tt. Некоторые языки проводят различие, например Текстиль, или позволить пользователю легко настроить вывод, например Texy.

LML иногда различаются разметкой из нескольких слов, где некоторые требуют, чтобы символы разметки заменяли межсловные пробелы (инфикс). Для некоторых языков требуется один символ в качестве префикса и суффикса, для других - удвоение или даже утроение или поддержка обоих символов с немного другим значением, например разные уровни акцента.

### Синтаксис заголовка

Заголовки обычно доступны на шести уровнях, но верхний часто зарезервирован для того, чтобы содержать то же самое, что и заголовок документа, который может быть установлен извне. В некоторых документах уровни могут быть связаны с типами подразделений, например часть, глава, раздел, статья или абзац.

Большинство языков LML следуют одному из двух стилей заголовков: либо Setext -подобное подчеркивание, или -подобные atx -подобные маркеры строки, либо они поддерживают оба стиля.
### Заголовки с префиксом
Второй стиль основан на повторяющихся маркерах (например, хэш #, равно =или звездочка *) в начале самого заголовка, где количество повторений указывает (иногда обратный) уровень заголовка. Большинство языков также поддерживают дублирование маркеров в конце строки, но в то время как некоторые делают их обязательными, другие даже не ожидают совпадения их номеров.

Microsoft Word поддерживает автоматическое форматирование абзацев в качестве заголовков, если они не содержат более нескольких слов, без точки в конце и если пользователь дважды нажимает клавишу ввода. Для более низких уровней пользователь может нажать клавишу табулятора соответствующее количество раз перед вводом текста, т. Е. С одной по восемь вкладок для уровней заголовков со второго по девятый.
### Синтаксис ссылки

Гиперссылки могут быть добавлены встроенными, что может загромождать код из-за длинных URL-адресов, либо с именованным псевдонимомили пронумерованным idссылки на строки, не содержащие ничего, кроме адреса и связанных атрибутов, и часто могут находиться в любом месте документа. Большинство языков позволяют автору указывать текст Textдля отображения вместо простого адреса http://example.com , а некоторые также предоставляют методы для установки другой заголовок ссылки Заголовок, который может содержать дополнительную информацию о месте назначения.

LML, предназначенные для особых настроек, например вики-страницы или документация по коду могут автоматически создавать именованные привязки (для заголовков, функций и т. д.) внутри документа, ссылаться на связанные страницы (возможно, в другом пространстве имен) или обеспечивать текстовый поиск связанных ключевых слов.

В большинстве языков для заключения ссылок используются (двойные) квадратные или угловые скобки, но вряд ли какие-либо два языка полностью совместимы. Многие могут автоматически распознавать и анализировать абсолютные URL-адреса внутри текста без дополнительной разметки.
### Синтаксис списка


HTML требует явного элемента для списка с указанием его типа и по одному для каждого элемента списка, но большинству облегченных языков разметки требуются только разные префиксы строк для маркеров или перечисленные элементы. Некоторые языки используют отступы для вложенных списков, другие используют повторяющиеся маркеры родительского списка.

