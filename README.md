# Cronexia / Test Next.js / avec Million / & Composants

Tout est dit

(si re-test, besoin de `bun i` ...)

## Installation

[doc](https://nextjs.org/docs/app/getting-started/installation)

```bash
# Auto via terminal // Rien à installer, probablement inclus dans node ou chp
npx create-next-app@latest

# Need to install the following packages:
# create-next-app@15.1.4
# Ok to proceed? (y) y

# ✔ What is your project named? … project
# ✔ Would you like to use TypeScript? … No / Yes
# ✔ Would you like to use ESLint? … No / Yes
# ✔ Would you like to use Tailwind CSS? … No / Yes
# ✔ Would you like your code inside a `src/` directory? … No / Yes
# ✔ Would you like to use App Router? (recommended) … No / Yes
# ✔ Would you like to use Turbopack for `next dev`? … No / Yes
# ✔ Would you like to customize the import alias (`@/*` by default)? … No / Yes

# ---

cd project/
bun dev
```

---

## Installation de Materials

~~[yay](https://github.com/material-components/material-web/blob/main/docs/quick-start.md)~~

[hoy](https://mui.com/material-ui/integrations/nextjs/)

```bash
# npm install @material/web
## bun i @material/web

# Manquait @emotion/react @emotion/styled
bun add @mui/material @mui/material-nextjs @emotion/cache @emotion/react @emotion/styled
```

Ajout de [boutons](https://mui.com/material-ui/react-button/) a la page de base. isOk

---

## Million

[hey](https://github.com/aidenybai/million)

Installation en suivant la doc (pour react...)

```bash
npx million@latest

# Need to install the following packages:
# million@3.1.11
# Ok to proceed? (y) y

# Need to install the following packages:
# @million/install@1.0.14
# Ok to proceed? (y) y

# ┌  ⚡ Million Lint
# │
# ◇  Do you want to use Million Lint in Visual Studio Code?
# │  Yes
# │
# ◇  Installed Visual Studio Code extension
# │
# ◆  Detected Next.js project.
# │
# ◇  Resolving dependencies
# Resolved, downloaded and extracted [628]
# Saved lockfile

# │
# ◇  Setup Million Lint in your next.config.ts?
# │  Yes
# │
# │
# ◇  Take a look at changes in project/next.config.ts ─╮
# │                                                    │
# │  import MillionLint from "@million/lint";          │
# │  import type { NextConfig } from "next";           │
# │  ...                                               │
# │                                                    │
# │  export default MillionLint.next({                 │
# │    enabled: true,                                  │
# │    rsc: true                                       │
# │  })(nextConfig);                                   │
# │                                                    │
# │                                                    │
# ├────────────────────────────────────────────────────╯
# ◇
# │
# ◇  Is the config file setup correctly?
# │  Yes
# │
# ◇  Add the .million/ directory to your .gitignore?
# │  Yes
# │
# ◇  Take a look at changes in /home/youpiwaza/code/cronexia-test-nextjs-w-million/.gitignore ─╮
# │                                                                                            │
#                                                                         │
# │                                                                                            │
# │  # Million Lint                                                                            │
# │  .million                                                                                  │
# │                                                                                            │
# │                                                                                            │
# ├────────────────────────────────────────────────────────────────────────────────────────────╯
# │
# └  ✓  You're all set!
```

❌📌 Test

 ⨯ ./src/app/layout.tsx
Error evaluating Node.js code
TypeError: 'process.env' only accepts a configurable, writable, and enumerable data descriptor

- ❌ au cas ou, article pour le [packer sur nestjs](https://dev.to/tobysolutions/how-to-use-millionjs-in-a-next-app-1eim)
  - HS

Vraie doc > [nextjs](https://million.dev/docs#manual-installation)

```bash
bun add @million/lint@latest
```

... et modifier la config, y'a trop rien en vrai

Tester sur une installation fraiche sans materials

HS également

mwé tester sur react directement ptet

[hey](https://create-react-app.dev/docs/getting-started)

```bash
npx create-react-app my-app
#  erreur a l'install, super
cd my-app

# Can't resolve 'web-vitals' // sans ça HMR HS
# Fixed
bun add web-vitals -d 
bun i

bun start
# isok

npx million@latest
```

Mwé ça fonctionne mais ça pète le HMR >_>

---

## Formulaires

Templates existants mais bon wala

[yay](https://mui.com/material-ui/getting-started/templates/#free-templates)

