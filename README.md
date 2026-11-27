# awesome-milkdown

🍼 A curated list of awesome things related to [Milkdown](https://milkdown.dev), the plugin-driven WYSIWYG Markdown editor framework.

[Website](https://milkdown.dev) · [GitHub](https://github.com/Milkdown/milkdown) · [Playground](https://milkdown.dev/playground)

<p align="center"><sub><b>USED IN PROJECTS FROM</b></sub></p>

<p align="center">
  <a href="#microsoft"><img src="assets/logos/microsoft.svg" alt="Microsoft" height="32"></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="#google-cloud"><img src="assets/logos/google-cloud.svg" alt="Google Cloud" height="26"></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="#tencent"><img src="assets/logos/tencent.svg" alt="Tencent" height="22"></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="#oracle"><img src="assets/logos/oracle.svg" alt="Oracle" height="18"></a>
</p>

<p align="center">
  <a href="#standard-notes"><img src="assets/logos/standard-notes.svg" alt="Standard Notes" height="30"></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="#teable"><img src="assets/logos/teable.svg" alt="Teable" height="44"></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="#marginnote"><img src="assets/logos/marginnote.svg" alt="MarginNote" height="32"></a>
</p>

## Contents

- [Official Packages](#official-packages)
- [Who's Using Milkdown](#whos-using-milkdown)
  - [Notable Organizations](#notable-organizations)
  - [More Projects](#more-projects)
- [Community Plugins & Integrations](#community-plugins--integrations)
- [Contributing](#contributing)

## Official Packages

All official packages live in the [Milkdown monorepo](https://github.com/Milkdown/milkdown/tree/main/packages).

### Getting Started

| name                                                             | description                                                                      |
| :--------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| [@milkdown/crepe](https://www.npmjs.com/package/@milkdown/crepe) | Ready-to-use editor with toolbar, slash menu, tables, LaTeX and more. Start here |
| [@milkdown/kit](https://www.npmjs.com/package/@milkdown/kit)     | An all-in-one package that re-exports core, presets, plugins and components      |
| [@milkdown/react](https://www.npmjs.com/package/@milkdown/react) | React integration                                                                |
| [@milkdown/vue](https://www.npmjs.com/package/@milkdown/vue)     | Vue integration                                                                  |

### Core

| name                                                                       | description                                                                |
| :------------------------------------------------------------------------- | :------------------------------------------------------------------------- |
| [@milkdown/core](https://www.npmjs.com/package/@milkdown/core)             | The editor kernel                                                          |
| [@milkdown/components](https://www.npmjs.com/package/@milkdown/components) | Prebuilt UI components: code block, image block, link tooltip, table, etc. |
| [@milkdown/theme-nord](https://www.npmjs.com/package/@milkdown/theme-nord) | A [Nord](https://www.nordtheme.com/) theme                                 |

### Presets & Plugins

| name                                                                                     | description                                                                    |
| :--------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| [@milkdown/preset-commonmark](https://www.npmjs.com/package/@milkdown/preset-commonmark) | Adds [CommonMark](https://commonmark.org/) syntax support                      |
| [@milkdown/preset-gfm](https://www.npmjs.com/package/@milkdown/preset-gfm)               | Adds [GFM](https://github.github.com/gfm/) syntax support                      |
| [@milkdown/plugin-history](https://www.npmjs.com/package/@milkdown/plugin-history)       | Undo & redo                                                                    |
| [@milkdown/plugin-clipboard](https://www.npmjs.com/package/@milkdown/plugin-clipboard)   | Markdown copy & paste                                                          |
| [@milkdown/plugin-listener](https://www.npmjs.com/package/@milkdown/plugin-listener)     | Listen to editor events such as `markdownUpdated`                              |
| [@milkdown/plugin-collab](https://www.npmjs.com/package/@milkdown/plugin-collab)         | Real-time collaborative editing with [Yjs](https://yjs.dev/)                   |
| [@milkdown/plugin-streaming](https://www.npmjs.com/package/@milkdown/plugin-streaming)   | Streams AI-generated Markdown into the document chunk by chunk                 |
| [@milkdown/plugin-diff](https://www.npmjs.com/package/@milkdown/plugin-diff)             | Diff review: compare two documents and accept or reject changes chunk by chunk |
| [@milkdown/plugin-block](https://www.npmjs.com/package/@milkdown/plugin-block)           | Block handle for dragging and operating on blocks                              |
| [@milkdown/plugin-slash](https://www.npmjs.com/package/@milkdown/plugin-slash)           | Slash command menus                                                            |
| [@milkdown/plugin-tooltip](https://www.npmjs.com/package/@milkdown/plugin-tooltip)       | Tooltips, e.g. a toolbar on text selection                                     |
| [@milkdown/plugin-automd](https://www.npmjs.com/package/@milkdown/plugin-automd)         | Turns inline Markdown syntax into formatting as you type                       |
| [@milkdown/plugin-highlight](https://www.npmjs.com/package/@milkdown/plugin-highlight)   | Code block highlighting with Shiki, lowlight, refractor or sugar-high          |
| [@milkdown/plugin-prism](https://www.npmjs.com/package/@milkdown/plugin-prism)           | Code block highlighting with [Prism](https://prismjs.com/)                     |
| [@milkdown/plugin-cursor](https://www.npmjs.com/package/@milkdown/plugin-cursor)         | Drop cursor & gap cursor                                                       |
| [@milkdown/plugin-trailing](https://www.npmjs.com/package/@milkdown/plugin-trailing)     | Keeps an empty paragraph at the end of the document                            |
| [@milkdown/plugin-emoji](https://www.npmjs.com/package/@milkdown/plugin-emoji)           | Emoji support                                                                  |
| [@milkdown/plugin-indent](https://www.npmjs.com/package/@milkdown/plugin-indent)         | Tab indentation                                                                |
| [@milkdown/plugin-upload](https://www.npmjs.com/package/@milkdown/plugin-upload)         | Drop & upload files                                                            |

## Who's Using Milkdown

### Notable Organizations

- <a name="microsoft"></a>**Microsoft**
  - [Huabu](https://github.com/microsoft/Huabu) - An infinite canvas where you and your agents think together. Notes and AI chat messages are edited with Crepe, and you can drag their blocks out onto the canvas.
  - [TypeAgent](https://github.com/microsoft/TypeAgent) - Sample code for a personal agent that works with application agents. Its markdown agent runs a Crepe editor synced over Yjs with `@milkdown/plugin-collab`, so you and the AI edit the same document.
- <a name="google-cloud"></a>**Google Cloud**
  - [Scion](https://github.com/GoogleCloudPlatform/scion) - An open-source orchestration platform for teams of AI agents. The Hub web UI uses Milkdown to review Markdown artifacts that agents publish, with suggestion and comment marks.
- <a name="tencent"></a>**Tencent**
  - [cherry-markdown](https://github.com/Tencent/cherry-markdown) - A Markdown editor. Its WYSIWYG mode, published as [@cherry-markdown/milkdown](https://www.npmjs.com/package/@cherry-markdown/milkdown), is built on Milkdown and reuses Cherry's parser, rendering and themes. The Cherry desktop client uses it too.
- <a name="oracle"></a>**Oracle**
  - [LiveSQL](https://livesql.oracle.com/landing/) - Instant access to Oracle Database, plus a collection of community scripts and tutorials.
- <a name="standard-notes"></a>**Standard Notes**
  - [Markdown Visual](https://github.com/standardnotes/plugins/tree/main/packages/com.sncommunity.markdown-visual) - A WYSIWYG Markdown editor plugin for Standard Notes, the end-to-end encrypted notes app. Built with Milkdown and published as [@standardnotes/markdown-visual](https://www.npmjs.com/package/@standardnotes/markdown-visual).
- <a name="teable"></a>**Teable**
  - [Teable](https://github.com/teableio/teable) - AI spreadsheet for business, and a no-code Airtable alternative built on Postgres. Long text fields are edited with Milkdown.
- <a name="marginnote"></a>**MarginNote**
  - [MarginNote-Milkdown](https://github.com/marginnoteapp/milkdown) - The official Markdown editor of [MarginNote](https://www.marginnote.com/), an e-reader for studying and digesting books.

### More Projects

#### Productivity & Data

- [TagSpaces](https://www.tagspaces.org/) - An offline, open-source file manager with tagging. Uses Milkdown to edit Markdown files.
- [ezone](https://ezone.work/) - 一站式云原生企业研发协同与效能平台 (an all-in-one, cloud-native R&D collaboration platform).

#### Markdown Editors & Note-Taking

- [milkdown-vscode](https://github.com/Saul-Mirone/milkdown-vscode) - Milkdown as the Markdown editor in VS Code.
- [GeekDown](https://github.com/fearlessgeekmedia/GeekDown) - A desktop Markdown editor powered by Milkdown.
- [type.](https://type.qurle.net) ([repo](https://github.com/qurle/type)) - A local-first zen editor with import, export and publishing.
- [standardnotes-milkdown](https://github.com/chuangzhu/standardnotes-milkdown) - A community Milkdown editor for [Standard Notes](https://standardnotes.com/).
- [Doclea](https://github.com/FalkZ/doclea) - An online document editor.

#### Other

- [typelog](https://typelog.dev) - A microblogging platform for developers. Posts and comments are written with Milkdown.
- [Howdz Dashboard](https://github.com/leon-kfd/Dashboard) - A browser start page built from configurable components.
- [vite-plugin-book](https://github.com/Saul-Mirone/vite-plugin-book) - A Vite plugin that generates and manages documentation websites. _(archived)_

## Community Plugins & Integrations

- [@cherry-markdown/milkdown](https://www.npmjs.com/package/@cherry-markdown/milkdown) - A WYSIWYG Milkdown editor that uses Cherry Markdown's parsing and themes, with ECharts, Mermaid and math renderers.
- [milkdown-plugin-file](https://github.com/omarmir/milkdown-plugin-file) - Adds remark directive support and a ProseMirror component for file uploads.
- [milkdown-mentions-plugin](https://github.com/zgrybus/milkdown-mentions-plugin) - Mention people and turn the mentions into links.
- [milkdown-plugin-image-picker](https://github.com/LittleSound/milkdown-plugin-image-picker) - Select and upload images from a file picker.
- [milkdown-plugin-placeholder](https://github.com/HexMox/milkdown-plugin-placeholder) - 🌈 A placeholder plugin.
- [milkdown-plugin-shiki](https://www.npmjs.com/package/milkdown-plugin-shiki) - Code block highlighting with [Shiki](https://shiki.style/).
- [@ezone-devops/milkdown-plugin-directive-fallback](https://www.npmjs.com/package/@ezone-devops/milkdown-plugin-directive-fallback) - Renders every directive as text, which avoids parse errors when using remark-directive.
- [@star-dancer/milkdown](https://www.npmjs.com/package/@star-dancer/milkdown) - Angular integration.
- [coditor](https://github.com/jiannei/coditor) - A collection of unofficial plugins, including placeholder, Shiki and a remote uploader.
- [milkdown-lab](https://github.com/enpitsuLin/milkdown-lab) - A collection of unofficial plugins, including [split editing](https://www.npmjs.com/package/@milkdown-lab/plugin-split-editing). _(archived)_

> Some community plugins were written for Milkdown v6 or earlier v7 releases. Check compatibility before using them.

## Contributing

Using Milkdown in your project, or built a plugin? Open a pull request that adds it to the right section, in this format:

```md
- [Name](link) - What it is, and how it uses Milkdown.
```

Organizations under [Notable Organizations](#notable-organizations) also appear in the logo wall at the top. If you represent one of them and want your logo updated or removed, please open an issue.
