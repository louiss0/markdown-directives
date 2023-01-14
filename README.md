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

| **Snippet** | **Purpose**                           |
| ----------- | ------------------------------------- |
| rmd-cd      | This is a container directive snippet |
| rmd-ld      | This is a leaf directive snippet      |
| rmd-td      | This is a text directive snippet      |

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
