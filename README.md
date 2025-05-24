# <div align="center"><div style="color:#448b5b;display:inline;">Effen</div> (by Aency)</div>

<div align="center">• English / <a href="https://github.com/aencyproject/readme-portuguese.md">Português</a> •</div>

<br>

<div style="color:#448b5b;display:inline;">Effen</div> ("<i>efficiency</i>" but abreviated in our way) is an all-in-one management tool for your system. The diference between Effen and other management tools is that Effen is designed to be as simple as possible, but super powerful and <a href="https://github.com/aencyproject/effen/README.md/#-what-can-effen-do">customizable</a>.

<br>

Check out the [CHANGELOG](CHANGELOG.md) for detailed updates, fixes and new features!

---

## 🎉 Effen 1.0

Effen 1.0 is the first release of Effen! It brings some basic features and a nice UI.

- Clean UI
- Functional UI
- Settings
- Basic Efferiums

---

## ✨ What can Effen do?

- ✅ **Functional multiplatform app**
- 💻 Fast, beautiful and clean interface
- 🎨 Accessibility and theme settings for better ease of use!
- 📝 Notes manager with options of Colors, Tags, Search, Export, Import, etc.
- 📂 File manager with options of Filtering, Types of View, Search, Rename in Mass, Colors, Tags.
- 🎵 Music player with options of Play, Pause, Stop, Volume, etc.
- 📊 System monitoring in real time, with performance graphs, process management, device management.
- 🖼️ Image gallery with options of Slides Presentation, Image Editing, Albums, Tags, Image Converter.

---

## Installation

To install, update or uninstall Effen, run one of the following commands according to your operating system below.

**Prerequisites**
- Node.js 23+
- PNPM 9+
- Git 2.47+
- Curl 8.11+ (Linuonly)

```bash
# Linux
curl -fsSL https://github.com/aencyproject/effen/raw/scripts/setup.sh | bash
```

---

## For Developers


- [React](https://react.dev/) - JavaScript library for building interfaces.
- [TailwindCSS](https://tailwindcss.com/) - Utility CSS framework.
- [Lucide Icons](https://lucide.dev/) - Modern icon package.
- [Vite](https://vitejs.dev/) - Build tool and dev server.
- [TypeScript](https://www.typescriptlang.org/) - Superset JavaScript tipado.
- [Shadcn/UI](https://ui.shadcn.com/) - Reusable React components.
- [Tauri](https://nwjs.io/) - Framework for creating desktop apps.


## 🛠️ Development Commands

| Command          | Description                              |
|------------------|----------------------------------------|
| pnpm build     | Creates a production build             |
| pnpm preview   | Previa a build localmente              |
| pnpm lint      | Lints the code                         |
| pnpm start | Inicia o aplicativo em modo de desenvolvimento |
| pnpm dev | Inicia o aplicativo em modo de desenvolvimento |

## 📚 Documentation
See the Effen documentation [here](https://effen.vercel.app/docs/)! Feel free to contribute at any time.

## 🤝 Contributors
A special thanks to all contributors who helped improve the app with your precious time! We love community contributions. Get started by reading our [CONTRIBUTING.md](CONTRIBUTING.md).<br>
> <img src="https://contrib.rocks/image?repo=aencyproject/effen" /><br>
> A special THANKS to [Roo Code](https://github.com/RooVetGit/Roo-Code/) for most of the README parts!

---

### Community

- **Discord:** [Join our Discord server](https://discord.gg/roocode) for real-time help and discussions
- **Reddit:** [Visit our subreddit](https://www.reddit.com/r/RooCode) to share experiences and tips
- **GitHub:** Report [issues](https://github.com/RooVetGit/Roo-Code/issues) or request [features](https://github.com/RooVetGit/Roo-Code/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop)










This is a [Tauri](https://v2.tauri.app/) project template using [Next.js](https://nextjs.org/),
bootstrapped by combining [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app)
and [`create tauri-app`](https://v2.tauri.app/start/create-project/).

This template uses [`pnpm`](https://pnpm.io/) as the Node.js dependency
manager, and uses the [App Router](https://nextjs.org/docs/app) model for Next.js.

## Template Features

- TypeScript frontend using [Next.js 15](https://nextjs.org/) React framework
- [TailwindCSS 4](https://tailwindcss.com/) as a utility-first atomic CSS framework
  - The example page in this template app has been updated to use only TailwindCSS
  - While not included by default, consider using
    [React Aria components](https://react-spectrum.adobe.com/react-aria/index.html)
    and/or [HeadlessUI components](https://headlessui.com/) for completely unstyled and
    fully accessible UI components, which integrate nicely with TailwindCSS
- Opinionated formatting and linting already setup and enabled
  - [Biome](https://biomejs.dev/) for a combination of fast formatting, linting, and
    import sorting of TypeScript code, and [ESLint](https://eslint.org/) for any missing
    Next.js linter rules not covered by Biome
  - [clippy](https://github.com/rust-lang/rust-clippy) and
    [rustfmt](https://github.com/rust-lang/rustfmt) for Rust code
- GitHub Actions to check code formatting and linting for both TypeScript and Rust

## Getting Started

```

To develop and run the frontend in a Tauri window:

```shell
pnpm tauri dev
```

This will load the Next.js frontend directly in a Tauri webview window, in addition to
starting a development server on `localhost:3000`.
Press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>I</kbd> in a Chromium based WebView (e.g. on
Windows) to open the web developer console from the Tauri window.

### Building for release

To export the Next.js frontend via SSG and build the Tauri application for release:

```shell
pnpm tauri build
```

### Source structure

Next.js frontend source files are located in `src/` and Tauri Rust application source
files are located in `src-tauri/`. Please consult the Next.js and Tauri documentation
respectively for questions pertaining to either technology.

## Caveats

### Static Site Generation / Pre-rendering

Next.js is a great React frontend framework which supports server-side rendering (SSR)
as well as static site generation (SSG or pre-rendering). For the purposes of creating a
Tauri frontend, only SSG can be used since SSR requires an active Node.js server.

Please read into the Next.js documentation for [Static Exports](https://nextjs.org/docs/app/building-your-application/deploying/static-exports)
for an explanation of supported / unsupported features and caveats.

### `next/image`

The [`next/image` component](https://nextjs.org/docs/basic-features/image-optimization)
is an enhancement over the regular `<img>` HTML element with server-side optimizations
to dynamically scale the image quality. This is only supported when deploying the
frontend onto Vercel directly, and must be disabled to properly export the frontend
statically. As such, the
[`unoptimized` property](https://nextjs.org/docs/api-reference/next/image#unoptimized)
is set to true for the `next/image` component in the `next.config.js` configuration.
This will allow the image to be served as-is, without changes to its quality, size,
or format.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and
  API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

And to learn more about Tauri, take a look at the following resources:

- [Tauri Documentation - Guides](https://v2.tauri.app/start/) - learn about the Tauri
  toolkit.
