# [Prism](https://prismjs.com/)


---
### **NOTE**
This is just a fork of `prismjs` package to fix worker issue on import and use inside a headless browser or ssr environment

---

[![npm](https://img.shields.io/npm/dw/@paranode/prismjs.svg)](https://www.npmjs.com/package/@paranode/prismjs)

Prism is a lightweight, robust, and elegant syntax highlighting library. It's a spin-off project from [Dabblet](https://dabblet.com/).

You can learn more on [prismjs.com](https://prismjs.com/).

[Why another syntax highlighter?](https://lea.verou.me/2012/07/introducing-prism-an-awesome-new-syntax-highlighter/#more-1841)

[More themes for Prism!](https://github.com/PrismJS/prism-themes)

## Contribute to Prism!

### **Important Notice**

We are currently working on [Prism v2](https://github.com/PrismJS/prism/discussions/3531) and will only accept security-relevant PRs for the time being.

Once work on Prism v2 is sufficiently advanced, we will accept PRs again. This will be announced on our [Discussion](https://github.com/PrismJS/prism/discussions) page and mentioned in the [roadmap discussion](https://github.com/PrismJS/prism/discussions/3531).

<details>
<summary>Prism v1 contributing notes</summary>

Prism depends on community contributions to expand and cover a wider array of use cases. If you like it, consider giving back by sending a pull request. Here are a few tips:

- Read the [documentation](https://prismjs.com/extending.html). Prism was designed to be extensible.
- Do not edit `prism.js`, it’s just the version of Prism used by the Prism website and is built automatically. Limit your changes to the unminified files in the `components/` folder. `prism.js` and all minified files are generated by our build system (see below).
- Use `npm ci` to install Prism's dependencies. Do not use `npm install` because it will cause non-deterministic builds.
- The build system uses [gulp](https://github.com/gulpjs/gulp) to minify the files and build `prism.js`. With all of Prism's dependencies installed, you just need to run the command `npm run build`.
- Please follow the code conventions used in the files already. For example, I use [tabs for indentation and spaces for alignment](http://lea.verou.me/2012/01/why-tabs-are-clearly-superior/). Opening braces are on the same line, closing braces on their own line regardless of construct. There is a space before the opening brace. etc etc.
- Please try to err towards more smaller PRs rather than a few huge PRs. If a PR includes changes that I want to merge and also changes that I don't, handling it becomes difficult.
- My time is very limited these days, so it might take a long time to review bigger PRs (small ones are usually merged very quickly), especially those modifying the Prism Core. This doesn't mean your PR is rejected.
- If you contribute a new language definition, you will be responsible for handling bug reports about that language definition.
- If you [add a new language definition](https://prismjs.com/extending.html#creating-a-new-language-definition) or plugin, you need to add it to `components.json` as well and rebuild Prism by running `npm run build`, so that it becomes available to the download build page. For new languages, please also add a few [tests](https://prismjs.com/test-suite.html) and an example in the `examples/` folder.
- Go to [prism-themes](https://github.com/PrismJS/prism-themes) if you want to add a new theme.

Thank you so much for contributing!!

### Software requirements

Prism will run on [almost any browser](https://prismjs.com/#features-full) and Node.js version but you need the following software to contribute:

- Node.js >= 10.x
- npm >= 6.x

</details>

## Translations

* [简体中文](https://www.awesomes.cn/repo/PrismJS/prism) (if unavailable, see [here](https://deepmind.t-salon.cc/article/113))
