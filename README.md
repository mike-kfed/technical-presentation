<img src="docs/logo.svg" style="margin-right: 10pt;width:100pt" align="right">
<h1>Technical Presentation</h1>

<br>
Make technical presentations in Markdown/HTML etc.

This is a fork of [`revealjs`](https://github.com/hakimel/reveal.js) with some modifications to
package to PDF and standalone HTML format. Also it includes a company `scss`
file for design modifications.

**See the [demo presentation here](https://gabyx.github.io/Technical-Presentation)**.

Authors: [Gabriel Nützi](https://github.com/gabyx) and [Simon Spörri](https://github.com/simonspoerri).

Current [`revealjs`](https://github.com/hakimel/reveal.js) version: `4.6.1`

## Examples

- `npm install` -> Install all dependencies.
- `npm run present` -> Presentation in Browser.
- `npm run package` -> PDF & HTML and standalone `zip` file to distribute.

## Modifications

- Edit design in [`company.scss`](css/theme/source/company.scss).
- Company Logo: Edit the file [`company-logo.svg`](css/theme/source/files/company-logo.svg).
- Replace embedded image in [`company.scss`](css/theme/source/company.scss) with

  ```shell
  repl=$(cat css/theme/source/files/company-logo.svg | base64 -w 0| sed "s/\+/\\\+/g")
  sed -i -E "s@background-image(.*);base64,.*\"@background-image\1;base64,$repl\"@" css/theme/source/company.scss
  ```

# RevealJS

<p align="center">
  <a href="https://revealjs.com">
  <img src="https://hakim-static.s3.amazonaws.com/reveal-js/logo/v1/reveal-black-text-sticker.png" alt="reveal.js" width="500">
  </a>
  <br><br>
  <a href="https://github.com/hakimel/reveal.js/actions"><img src="https://github.com/hakimel/reveal.js/workflows/tests/badge.svg"></a>
  <a href="https://slides.com/"><img src="https://s3.amazonaws.com/static.slid.es/images/slides-github-banner-320x40.png?1" alt="Slides" width="160" height="20"></a>
</p>

reveal.js is an open source HTML presentation framework. It enables anyone with a web browser to create beautiful presentations for free. Check out the live demo at [revealjs.com](https://revealjs.com/).

The framework comes with a powerful feature set including [nested slides](https://revealjs.com/vertical-slides/), [Markdown support](https://revealjs.com/markdown/), [Auto-Animate](https://revealjs.com/auto-animate/), [PDF export](https://revealjs.com/pdf-export/), [speaker notes](https://revealjs.com/speaker-view/), [LaTeX typesetting](https://revealjs.com/math/), [syntax highlighted code](https://revealjs.com/code/) and an [extensive API](https://revealjs.com/api/).

---

Want to create reveal.js presentation in a graphical editor? Try <https://slides.com>. It's made by the same people behind reveal.js.

---

### Sponsors

Hakim's open source work is supported by <a href="https://github.com/sponsors/hakimel">GitHub sponsors</a>. Special thanks to:

<div align="center">
  <table>
    <td align="center">
      <a href="https://workos.com/?utm_campaign=github_repo&utm_medium=referral&utm_content=revealjs&utm_source=github">
        <div>
          <img src="https://user-images.githubusercontent.com/629429/151508669-efb4c3b3-8fe3-45eb-8e47-e9510b5f0af1.svg" width="290" alt="WorkOS">
        </div>
        <b>Your app, enterprise-ready.</b>
        <div>
          <sub>Start selling to enterprise customers with just a few lines of code. Add Single Sign-On (and more) in minutes instead of months.</sup>
        </div>
      </a>
    </td>
  </table>
</div>

---

### Getting started

- 🚀 [Install reveal.js](https://revealjs.com/installation)
- 👀 [View the demo presentation](https://revealjs.com/demo)
- 📖 [Read the documentation](https://revealjs.com/markup/)
- 🖌 [Try the visual editor for reveal.js at Slides.com](https://slides.com/)
- 🎬 [Watch the reveal.js video course (paid)](https://revealjs.com/course)

---

<div align="center">
  MIT licensed | Copyright © 2011-2023 Hakim El Hattab, https://hakim.se
</div>
