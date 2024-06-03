
Below is a complex example of Markdown showcasing various elements such as code blocks, tables, images, and more:

H~2~O



# Complex Markdown Example

## Code Blocks
You can display code blocks in Markdown by using triple backticks. You can also specify the programming language for syntax highlighting.



- ```python
def greet(name):
    print(f"Hello, {name}!")
```
    - ```javascript
const add = (a, b) => a + b;
```

## Tables with code blocks, links, and media
Tables can be created using pipes and hyphens.

| Name      | Age | Occupation   |
|-----------|-----|--------------|
| > John      | ~~30~~  | ```python    |
| ```javascript  | 25  | [Google](https://www.google.com)     |
| **Michael**   | 40  | ![Nature](https://thumbs.dreamstime.com/z/bee-flower-27533578.jpg)    |

## Images
You can embed images using

![Nature](https://thumbs.dreamstime.com/z/bee-flower-27533578.jpg)

## Links
You can create hyperlinks using `[link text](URL)` syntax.

Here's a link to [Google](https://www.google.com).

## Text Formatting
You can add formatting to your text:

- **Bold**: Wrap the text in double asterisks or underscores: `**bold text**` or `__bold text__`.
- *Italic*: Wrap the text in single asterisks or underscores: `*italic text*` or `_italic text_`.
- ~~Strikethrough~~: Use double tilde: `~~strikethrough text~~`.

## Lists
You can create ordered and unordered lists.

Unordered list:
- Item 1
- Item 2
- Item 3

Ordered list:
1. First item
2. Second item
3. Third item

## Blockquotes
You can create blockquotes using the greater than sign (\>) at the start of the line.

> This is a blockquote.
> It can span multiple lines.

## Horizontal Rule
You can add a horizontal rule using three hyphens, underscores, or asterisks.

---

## Escaping Characters
To display special characters as plain text, use a backslash (\) before the character.

For example, \*This text will not be italicized\*.

# Comparison of syntax extensions in Markdown flavors 

I created a crude comparison of the syntax of the various common Markdown extensions to have a better view on what are the most common extensions and what is the most widely accepted syntax for them. The list of Markdown flavors that I looked at was based on the list found on CommonMark's [GitHub Wiki](https://github.com/commonmark/commonmark/wiki/markdown-flavors).

| Flavor            |    Superscript    | Subscript | Deletion*<br>Strikethrough | Insertion*  | Highlight*  |  Footnote  |  Task list   | Table |      Abbr       | Deflist | Smart typo |    TOC    |                Math                 |              Math Block               | Mermaid |
| ----------------- | :---------------: | :-------: | :------------------------: | :---------: | :---------: | :--------: | :----------: | :---: | :-------------: | :-----: | :--------: | :-------: | :---------------------------------: | :-----------------------------------: | :-----: |
| GFM               |                   |           |         `~~...~~`          |             |             |            |  `- [] ...`  |   +   |                 |         |            |           |                                     |                                       |         |
| **ExtraMark**     |      `^...^`      |  `~...~`  |        `{--...--}`         | `{++...++}` | `{==...==}` | `[^...]`** | `- [] ...`** |   +   | `*[...]: ...`** |  `: `   |            |           |                                     |                                       |         |
| MultiMarkdown     | `^...^`<br>`^...` |  `~...~`  |        `{--...--}`         | `{++...++}` | `{==...==}` |  `[^...]`  |              |   +   |  `*[...]: ...`  |  `: `   |     +      | `{{TOC}}` |             `\\(...\\)`             |              `\\[...\\]`              |         |
| Markdown Extra    |                   |           |                            |             |             |   `[^1]`   |              |   +   |  `*[...]: ...`  |  `: `   |            |           |                                     |                                       |         |
| Pandoc            |      `^...^`      |  `~...~`  |         `~~...~~`          |             |             |  `[^...]`  |              |   +   |  `*[...]: ...`  |  `: `   |            |           |               `$...$`               |                                       |         |
| Kramdown          |                   |           |                            |             |             |   `[^1]`   |              |   +   |  `*[...]: ...`  |  `: `   |            |           |                                     |                                       |         |
| Markua            |      `^...^`      |  `~...~`  |  `~~...~~`<br>`{--...--}`  | `{++...++}` | `{==...==}` |  `[^...]`  |              |   +   |                 |  `: `   |            |           |            `` `...`$ ``             |                                       |         |
| Maruku            |                   |           |                            |             |             |   `[^1]`   |              |   +   |  `*[...]: ...`  |  `: `   |            |           |               `$...$`               |                 `$$`                  |         |
| Markdown2         |      `^...^`      |           |                            |             |             |            |              |   +   |                 |         |            |           |                                     |                                       |         |
| Remarkable        |      `^...^`      |  `~...~`  |         `~~...~~`          |  `++...++`  |  `==...==`  |            |              |       |                 |         |     +      |           |                                     |                                       |         |
| Showdown          |                   |           |         `~~...~~`          |             |             |   `[^1]`   |  `- [] ...`  |   +   |                 |         |            |  `[toc]`  | `$ ... $`<br>`~...~`<br>`\\(...\\)` | `\\[...\\]`<br>```` ```asciimath ```` |         |
| Ghost             |      `^...^`      |  `~...~`  |         `~~...~~`          |             |  `==...==`  |            |              |       |                 |         |            |           |                                     |                                       |         |
| GitLab            |                   |           |  `~~...~~`<br>`{- ... -}`  | `{+ ... +}` |             |   `[^1]`   |  `- [] ...`  |   +   |                 |         |            |           |               `$...$`               |           ```` ```math ````           |    +    |
| Haroopad          |                   |           |                            |             |  `==...==`  |            |  `- [] ...`  |       |                 |         |            |  `[TOC]`  |                                     |                                       |    +    |
| iA Writer         |                   |           |                            |             |             |   `[^1]`   |  `- [] ...`  |   +   |                 |         |            | `{{TOC}}` |       `$...$`<br>`\\(...\\)`        |       `$$...$$`<br>`\\[...\\]`        |         |
| Redcarpet         |     `^(...)`      |           |         `~~...~~`          |             |  `==...==`  |   `[^1]`   |              |   +   |                 |         |            |           |                                     |                                       |         |
| ScholarlyMarkdown |                   |           |                            |             |             |            |              |       |                 |         |            |           |     `$...$`<br>``` ``....`` ```     |           ```` ```math ````           |         |
| Taiga             |                   |           |                            |             |             |            |              |   +   |                 |         |            |           |                                     |                                       |         |
| Trello            |                   |           |         `~~...~~`          |             |             |            |              |       |                 |         |            |           |                                     |                                       |         |
| s9e\TextFormatter | `^...^`<br>`^...` |  `~...~`  |         `~~...~~`          |             |             |            |              |       |                 |         |            |           |                                     |                                       |         |

`[*]`: Some dialects use the [CriticMarkup] syntax for these features
`[**]`: Planned in the future

[CriticMarkup]: http://criticmarkup.com

# The markdown below is not supported by the editor

## Task Lists
You can create task lists by using brackets with spaces [ ], [x], or [X].

- [x] Task 1
- [ ] Task 2
- [ ] Task 3

## Footnotes
You can add footnotes using the caret and brackets syntax [^1].

[^1]: This is a footnote.



## LaTeX Equations
You can include mathematical equations using LaTeX syntax.

Inline equation: \(E = mc^2\)

Display equation:
\[F(x) = \int_{-\infty}^{\infty} f(x) \, dx\]

## YouTube Videos
You can embed YouTube videos using an iframe.

<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>

## Emoji
You can include emoji using colons like :smile: or :rocket:.

## Check GitHub Markdown Guide
For more advanced Markdown features, check the [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/).


This example showcases various elements in Markdown, including code blocks, tables, images, links, text formatting, lists, blockquotes, horizontal rule, task lists, footnotes, escaping characters, LaTeX equations, YouTube videos, and emojis. You can render this Markdown code in a Markdown editor or a platform that supports Markdown rendering to see the output.























This is how i understand whats happening:

    Markdown has syntax where 4 spaces equals a code blockI've just been exploring this within GitHubs markdown editor. Having four spaces in the markdown syntax -> pasting that markdown into our editor -> doesn't cause a code block to be added. 

New line
Shift enter
    4 spaces no code block

    4 spaces
    end

Clear

# markdown-it <!-- omit in toc -->

[![CI](https://github.com/markdown-it/markdown-it/workflows/CI/badge.svg)](https://github.com/markdown-it/markdown-it/actions)
[![NPM version](https://img.shields.io/npm/v/markdown-it.svg?style=flat)](https://www.npmjs.org/package/markdown-it)
[![Coverage Status](https://coveralls.io/repos/markdown-it/markdown-it/badge.svg?branch=master&service=github)](https://coveralls.io/github/markdown-it/markdown-it?branch=master)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/markdown-it/markdown-it)

> Markdown parser done right. Fast and easy to extend.

__[Live demo](https://markdown-it.github.io)__

- Follows the __[CommonMark spec](http://spec.commonmark.org/)__ + adds syntax extensions & sugar (URL autolinking, typographer).
- Configurable syntax! You can add new rules and even replace existing ones.
- High speed.
- [Safe](https://github.com/markdown-it/markdown-it/tree/master/docs/security.md) by default.
- Community-written __[plugins](https://www.npmjs.org/browse/keyword/markdown-it-plugin)__ and [other packages](https://www.npmjs.org/browse/keyword/markdown-it) on npm.

__Table of content__

- [Install](#install)
- [Usage examples](#usage-examples)
  - [Simple](#simple)
  - [Init with presets and options](#init-with-presets-and-options)
  - [Plugins load](#plugins-load)
  - [Syntax highlighting](#syntax-highlighting)
  - [Linkify](#linkify)
- [API](#api)
- [Syntax extensions](#syntax-extensions)
  - [Manage rules](#manage-rules)
- [Benchmark](#benchmark)
- [markdown-it for enterprise](#markdown-it-for-enterprise)
- [Authors](#authors)
- [References / Thanks](#references--thanks)

## Install

**node.js**:

```bash
npm install markdown-it --save
```

**browser (CDN):**

- [jsDeliver CDN](http://www.jsdelivr.com/#!markdown-it "jsDelivr CDN")
- [cdnjs.com CDN](https://cdnjs.com/libraries/markdown-it "cdnjs.com")




## Usage examples

See also:

- __[API documentation](https://markdown-it.github.io/markdown-it/)__ - for more
  info and examples.
- [Development info](https://github.com/markdown-it/markdown-it/tree/master/docs) -
  for plugins writers.


### Simple

```js
// node.js, "classic" way:
var MarkdownIt = require('markdown-it'),
    md = new MarkdownIt();
var result = md.render('# markdown-it rulezz!');

// node.js, the same, but with sugar:
var md = require('markdown-it')();
var result = md.render('# markdown-it rulezz!');

// browser without AMD, added to "window" on script load
// Note, there is no dash in "markdownit".
var md = window.markdownit();
var result = md.render('# markdown-it rulezz!');
```

Single line rendering, without paragraph wrap:

```js
var md = require('markdown-it')();
var result = md.renderInline('__markdown-it__ rulezz!');
```


### Init with presets and options

(*) presets define combinations of active rules and options. Can be
`"commonmark"`, `"zero"` or `"default"` (if skipped). See
[API docs](https://markdown-it.github.io/markdown-it/#MarkdownIt.new) for more details.

```js
// commonmark mode
var md = require('markdown-it')('commonmark');

// default mode
var md = require('markdown-it')();

// enable everything
var md = require('markdown-it')({
  html: true,
  linkify: true,
  typographer: true
});

// full options list (defaults)
var md = require('markdown-it')({
  html:         false,        // Enable HTML tags in source
  xhtmlOut:     false,        // Use '/' to close single tags (<br />).
                              // This is only for full CommonMark compatibility.
  breaks:       false,        // Convert '\n' in paragraphs into <br>
  langPrefix:   'language-',  // CSS language prefix for fenced blocks. Can be
                              // useful for external highlighters.
  linkify:      false,        // Autoconvert URL-like text to links

  // Enable some language-neutral replacement + quotes beautification
  // For the full list of replacements, see https://github.com/markdown-it/markdown-it/blob/master/lib/rules_core/replacements.js
  typographer:  false,

  // Double + single quotes replacement pairs, when typographer enabled,
  // and smartquotes on. Could be either a String or an Array.
  //
  // For example, you can use '«»„“' for Russian, '„“‚‘' for German,
  // and ['«\xA0', '\xA0»', '‹\xA0', '\xA0›'] for French (including nbsp).
  quotes: '“”‘’',

  // Highlighter function. Should return escaped HTML,
  // or '' if the source string is not changed and should be escaped externally.
  // If result starts with <pre... internal wrapper is skipped.
  highlight: function (/*str, lang*/) { return ''; }
});
```

### Plugins load

```js
var md = require('markdown-it')()
            .use(plugin1)
            .use(plugin2, opts, ...)
            .use(plugin3);
```


### Syntax highlighting

Apply syntax highlighting to fenced code blocks with the `highlight` option:

```js
var hljs = require('highlight.js'); // https://highlightjs.org

// Actual default values
var md = require('markdown-it')({
  highlight: function (str, lang) {
    if (lang && hljs.getLanguage(lang)) {
      try {
        return hljs.highlight(str, { language: lang }).value;
      } catch (__) {}
    }

    return ''; // use external default escaping
  }
});
```

Or with full wrapper override (if you need assign class to `<pre>`):

```js
var hljs = require('highlight.js'); // https://highlightjs.org

// Actual default values
var md = require('markdown-it')({
  highlight: function (str, lang) {
    if (lang && hljs.getLanguage(lang)) {
      try {
        return '<pre class="hljs"><code>' +
               hljs.highlight(str, { language: lang, ignoreIllegals: true }).value +
               '</code></pre>';
      } catch (__) {}
    }

    return '<pre class="hljs"><code>' + md.utils.escapeHtml(str) + '</code></pre>';
  }
});
```

### Linkify

`linkify: true` uses [linkify-it](https://github.com/markdown-it/linkify-it). To
configure linkify-it, access the linkify instance through `md.linkify`:

```js
md.linkify.set({ fuzzyEmail: false });  // disables converting email to link
```


## API

__[API documentation](https://markdown-it.github.io/markdown-it/)__

If you are going to write plugins, please take a look at
[Development info](https://github.com/markdown-it/markdown-it/tree/master/docs).


## Syntax extensions

Embedded (enabled by default):

- [Tables](https://help.github.com/articles/organizing-information-with-tables/) (GFM)
- [Strikethrough](https://help.github.com/articles/basic-writing-and-formatting-syntax/#styling-text) (GFM)

Via plugins:

- [subscript](https://github.com/markdown-it/markdown-it-sub)
- [superscript](https://github.com/markdown-it/markdown-it-sup)
- [footnote](https://github.com/markdown-it/markdown-it-footnote)
- [definition list](https://github.com/markdown-it/markdown-it-deflist)
- [abbreviation](https://github.com/markdown-it/markdown-it-abbr)
- [emoji](https://github.com/markdown-it/markdown-it-emoji)
- [custom container](https://github.com/markdown-it/markdown-it-container)
- [insert](https://github.com/markdown-it/markdown-it-ins)
- [mark](https://github.com/markdown-it/markdown-it-mark)
- ... and [others](https://www.npmjs.org/browse/keyword/markdown-it-plugin)


### Manage rules

By default all rules are enabled, but can be restricted by options. On plugin
load all its rules are enabled automatically.

```js
// Activate/deactivate rules, with currying
var md = require('markdown-it')()
            .disable([ 'link', 'image' ])
            .enable([ 'link' ])
            .enable('image');

// Enable everything
md = require('markdown-it')({
  html: true,
  linkify: true,
  typographer: true,
});
```

You can find all rules in sources:

- [`parser_core.js`](lib/parser_core.js)
- [`parser_block.js`](lib/parser_block.js)
- [`parser_inline.js`](lib/parser_inline.js)


## Benchmark

Here is the result of readme parse at MB Pro Retina 2013 (2.4 GHz):

```bash
make benchmark-deps
benchmark/benchmark.js readme

Selected samples: (1 of 28)
 > README

Sample: README.md (7774 bytes)
 > commonmark-reference x 1,222 ops/sec ±0.96% (97 runs sampled)
 > current x 743 ops/sec ±0.84% (97 runs sampled)
 > current-commonmark x 1,568 ops/sec ±0.84% (98 runs sampled)
 > marked x 1,587 ops/sec ±4.31% (93 runs sampled)
```

__Note.__ CommonMark version runs with [simplified link normalizers](https://github.com/markdown-it/markdown-it/blob/master/benchmark/implementations/current-commonmark/index.js)
for more "honest" compare. Difference is ≈1.5×.

As you can see, `markdown-it` doesn't pay with speed for its flexibility.
Slowdown of "full" version caused by additional features not available in
other implementations.


## markdown-it for enterprise

Available as part of the Tidelift Subscription.

The maintainers of `markdown-it` and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source dependencies you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainers of the exact dependencies you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-markdown-it?utm_source=npm-markdown-it&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)


## Authors

- Alex Kocharin [github/rlidwka](https://github.com/rlidwka)
- Vitaly Puzrin [github/puzrin](https://github.com/puzrin)

_markdown-it_ is the result of the decision of the authors who contributed to
99% of the _Remarkable_ code to move to a project with the same authorship but
new leadership (Vitaly and Alex). It's not a fork.

## References / Thanks

Big thanks to [John MacFarlane](https://github.com/jgm) for his work on the
CommonMark spec and reference implementations. His work saved us a lot of time
during this project's development.

**Related Links:**

- https://github.com/jgm/CommonMark - reference CommonMark implementations in C & JS,
  also contains latest spec & online demo.
- http://talk.commonmark.org - CommonMark forum, good place to collaborate
  developers' efforts.

**Ports**

- [motion-markdown-it](https://github.com/digitalmoksha/motion-markdown-it) - Ruby/RubyMotion
- [markdown-it-py](https://github.com/ExecutableBookProject/markdown-it-py)- Python
