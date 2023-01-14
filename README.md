# Remark HTML Directives

This is a set of snippets to use with the plugin [Remark HTML Directives](https://www.npmjs.com/package/remark-html-directives). If you install the plugin then you can then use this extension to get rid of lots of boilerplate code and become productive. For those who don't know what a  markdown directive is. A markdown directive is a directive that allows you to create HTML in the form of tags that are prefixed with a colon.

- One colon is a text directive
- Two colons is a leaf directive
- Three colons is a container directive

When it comes to directives you can add attributes to them and those turn into HTML attributes. They give nice shorthand's as well. Your Markdown is basically turned into a Templating Language. The term `rmd` is a keyword called Remark Markdown Directives. Anything post fixed with d is a directive.

## Installation

**Either**

- click the extensions button (lowest square icon in the editor), and type in Remark HTML Directives Snippets, select the one by Shelton Louis
- go to the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=SheltonLouis.remark-html-directives)

## Features

Below is all of the directives that are supported by this plugin.

### Core directives

| **Snippet** | **Purpose**                           |
| ----------- | ------------------------------------- |
| rmd-cd      | This is a container directive snippet |
| rmd-ld      | This is a leaf directive snippet      |
| rmd-td      | This is a text directive snippet      |

### Container directives

| **Snippet** | **Purpose**                                 |
| ----------- | ------------------------------------------- |
| rmd-hd      | This is a header directive snippet          |
| rmd-m       | This is a main directive snippet            |
| rmd-ft      | This is a footer directive snippet          |
| rmd-st      | This is a section directive snippet         |
| rmd-fg      | This is a figure directive snippet          |
| rmd-adr     | This is a address directive snippet         |
| rmd-as      | This is a aside directive snippet           |
| rmd-bq      | This is a blockquote directive snippet      |
| rmd-dts     | This is a details directive snippet         |
| rmd-smr     | This is a summary directive snippet         |
| rmd-dfl     | This is a definition list directive snippet |
| rmd-fc      | This is a figcaption directive snippet      |
| rmd-hr      | This is a horizontal rule directive snippet |
| rmd-li      | This is a list item directive snippet       |
| rmd-nav     | This is a navigation list directive snippet |
| rmd-ol      | This is a Ordered List directive snippet    |
| rmd-ul      | This is a Unordered List directive snippet  |
| rmd-vd      | This is a video directive snippet           |
| rmd-ad      | This is a audio directive snippet           |
| rmd-hg      | This is a hgroup directive snippet          |
| rmd-tb      | This is a table directive snippet           |
| rmd-tdh     | This is a table header directive snippet    |
| rmd-tbf     | This is a table footer directive snippet    |
| rmd-tbbd    | This is a table body directive snippet      |
| rmd-tbh     | This is a table head directive snippet      |
| rmd-tbhd    | This is a table header directive snippet    |
| rmd-tr      | This is a table row directive snippet       |
| rmd-tbdc    | This is a table data cell directive snippet |
| rmd-cl      | This is a column directive snippet          |
| rmd-ct      | This is a caption directive snippet         |
| rmd-cg      | This is a colgroup directive snippet        |
| rmd-cde     | This is a code directive snippet            |

### Leaf directives

| **Snippet** | **Purpose**                            |
| ----------- | -------------------------------------- |
| rmd-br      | This is a Break Rule directive snippet |
| rmd-img     | This is a Image directive snippet      |
| rmd-map     | This is a map directive snippet        |
| rmd-if      | This is a iframe directive snippet     |

### Text directives

| **Snippet** | **Purpose**                                         |
| ----------- | --------------------------------------------------- |
| rmd-ct      | This is a cite directive snippet                    |
| rmd-dfn     | This is a Definition directive snippet              |
| rmd-sb      | This is a subscript directive snippet               |
| rmd-sp      | This is a superscript directive snippet             |
| rmd-tm      | This is a time directive snippet                    |
| rmd-v       | This is a var directive snippet                     |
| rmd-mk      | This is a mark directive snippet                    |
| rmd-sml     | This is a small directive snippet                   |
| rmd-kbd     | This is a keyboard directive snippet                |
| rmd-smp     | This is a sample output directive snippet           |
| rmd-abbr    | This is a Abbreviation directive snippet            |
| rmd-bdo     | This is a bi-directional override directive snippet |
| rmd-data    | This is a data directive snippet                    |
| rmd-dt      | This is a definition term directive snippet         |
| rmd-dd      | This is a definition description directive snippet  |

## Requirements

You don't need any markdown specific tooling to use this extension. But since it is based of the `remark-html-directives` plugin that I created the rules that apply to that plugin will apply to these set of snippets.

<br>

> [!warning]  
> You can't use any HTML that is does not belong exclusively to the body tag.
> This plugin is based of the idea that you use a static site generator. They use either the concept of Injected layouts of they use Component's that wrap Markdown inside of a body tag.

<br>

**To use them in a project you will have to do this.**

```
pnpm i -D remark-directive remark-html-directives
```

**Then do this.**

```
{
	plugins: [
	    "remark-directive",
	    "remark-html-directives"
	],
}
```

> [!warning] Attention
> The remark-directive plugin must always be run before the remark-html-directives plugin is they rely on each other. remark-html-directives is a plugin that tells remark-directive how to work.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

Initial release of ...Remark HTML Directive Snippets.

<!-- ### 1.0.1

Fixed issue #.

### 1.1.0


Added features X, Y, and Z.



--- -->

## Post Statement

I recommend using [Astro.js](https://docs.astro.build/en/getting-started). You won't regret it. It will become the Figma of Static Site Generators in years to come.
