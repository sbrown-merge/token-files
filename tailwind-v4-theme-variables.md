# Tailwind CSS v4 Theme Variables Reference

This is a complete listing of Tailwind CSS v4 (v4.3) theme variables. Dimensional namespaces (type, spacing, sizing, radius, etc.) include REM-to-pixel conversions calculated at the default 16px root font size. All values are taken from the canonical default `theme.css` shipped with `tailwindcss`.

## Namespaces (overview)

Each namespace maps to one or more utility class or variant APIs. Defining a new variable within a namespace generates the corresponding utility automatically.

| Namespace | Generates |
|---|---|
| `--color-*` | Color utilities (`bg-*`, `text-*`, `fill-*`, etc.) |
| `--font-*` | Font family utilities (`font-sans`) |
| `--text-*` | Font size utilities (`text-xl`) |
| `--font-weight-*` | Font weight utilities (`font-bold`) |
| `--tracking-*` | Letter spacing (`tracking-wide`) |
| `--leading-*` | Line height (`leading-tight`) |
| `--breakpoint-*` | Responsive variants (`sm:*`) |
| `--container-*` | Container query variants + `max-w-*` |
| `--spacing-*` | Spacing/sizing utilities (`px-4`, `max-h-16`) |
| `--radius-*` | Border radius (`rounded-sm`) |
| `--shadow-*` | Box shadow (`shadow-md`) |
| `--inset-shadow-*` | Inset box shadow |
| `--drop-shadow-*` | Drop shadow filter |
| `--text-shadow-*` | Text shadow |
| `--blur-*` | Blur filter |
| `--perspective-*` | Perspective |
| `--aspect-*` | Aspect ratio |
| `--ease-*` | Transition timing |
| `--animate-*` | Animation |

## Spacing

The spacing scale is generated dynamically from a single base value; spacing and sizing utilities multiply this base.

| Variable | REM | Pixels |
|---|---|---|
| `--spacing` | 0.25rem | 4px |

## Font size (`--text-*`)

Each font size ships with a paired default line-height defined as a `calc()` ratio.

| Variable | REM | Pixels | Default line-height |
|---|---|---|---|
| `--text-xs` | 0.75rem | 12px | calc(1 / 0.75) ≈ 1rem / 16px |
| `--text-sm` | 0.875rem | 14px | calc(1.25 / 0.875) ≈ 1.25rem / 20px |
| `--text-base` | 1rem | 16px | calc(1.5 / 1) = 1.5rem / 24px |
| `--text-lg` | 1.125rem | 18px | calc(1.75 / 1.125) ≈ 1.75rem / 28px |
| `--text-xl` | 1.25rem | 20px | calc(1.75 / 1.25) ≈ 1.75rem / 28px |
| `--text-2xl` | 1.5rem | 24px | calc(2 / 1.5) ≈ 2rem / 32px |
| `--text-3xl` | 1.875rem | 30px | calc(2.25 / 1.875) ≈ 2.25rem / 36px |
| `--text-4xl` | 2.25rem | 36px | calc(2.5 / 2.25) ≈ 2.5rem / 40px |
| `--text-5xl` | 3rem | 48px | 1 |
| `--text-6xl` | 3.75rem | 60px | 1 |
| `--text-7xl` | 4.5rem | 72px | 1 |
| `--text-8xl` | 6rem | 96px | 1 |
| `--text-9xl` | 8rem | 128px | 1 |

## Breakpoints (`--breakpoint-*`)

| Variable | REM | Pixels |
|---|---|---|
| `--breakpoint-sm` | 40rem | 640px |
| `--breakpoint-md` | 48rem | 768px |
| `--breakpoint-lg` | 64rem | 1024px |
| `--breakpoint-xl` | 80rem | 1280px |
| `--breakpoint-2xl` | 96rem | 1536px |

## Containers (`--container-*`)

| Variable | REM | Pixels |
|---|---|---|
| `--container-3xs` | 16rem | 256px |
| `--container-2xs` | 18rem | 288px |
| `--container-xs` | 20rem | 320px |
| `--container-sm` | 24rem | 384px |
| `--container-md` | 28rem | 448px |
| `--container-lg` | 32rem | 512px |
| `--container-xl` | 36rem | 576px |
| `--container-2xl` | 42rem | 672px |
| `--container-3xl` | 48rem | 768px |
| `--container-4xl` | 56rem | 896px |
| `--container-5xl` | 64rem | 1024px |
| `--container-6xl` | 72rem | 1152px |
| `--container-7xl` | 80rem | 1280px |

## Border radius (`--radius-*`)

| Variable | REM | Pixels |
|---|---|---|
| `--radius-xs` | 0.125rem | 2px |
| `--radius-sm` | 0.25rem | 4px |
| `--radius-md` | 0.375rem | 6px |
| `--radius-lg` | 0.5rem | 8px |
| `--radius-xl` | 0.75rem | 12px |
| `--radius-2xl` | 1rem | 16px |
| `--radius-3xl` | 1.5rem | 24px |
| `--radius-4xl` | 2rem | 32px |

## Blur (`--blur-*`)

Blur values are defined natively in pixels.

| Variable | Pixels |
|---|---|
| `--blur-xs` | 4px |
| `--blur-sm` | 8px |
| `--blur-md` | 12px |
| `--blur-lg` | 16px |
| `--blur-xl` | 24px |
| `--blur-2xl` | 40px |
| `--blur-3xl` | 64px |

## Perspective (`--perspective-*`)

Perspective values are defined natively in pixels.

| Variable | Pixels |
|---|---|
| `--perspective-dramatic` | 100px |
| `--perspective-near` | 300px |
| `--perspective-normal` | 500px |
| `--perspective-midrange` | 800px |
| `--perspective-distant` | 1200px |

## Non-dimensional variables

The following namespaces use units other than REM/px (em, unitless, ratios) or use composite/keyword values.

### Font families

`--font-sans`, `--font-serif`, `--font-mono` — each is a full font stack.

### Font weights (`--font-weight-*`)

| Variable | Value |
|---|---|
| `--font-weight-thin` | 100 |
| `--font-weight-extralight` | 200 |
| `--font-weight-light` | 300 |
| `--font-weight-normal` | 400 |
| `--font-weight-medium` | 500 |
| `--font-weight-semibold` | 600 |
| `--font-weight-bold` | 700 |
| `--font-weight-extrabold` | 800 |
| `--font-weight-black` | 900 |

### Letter spacing (`--tracking-*`, em-based)

| Variable | Value |
|---|---|
| `--tracking-tighter` | -0.05em |
| `--tracking-tight` | -0.025em |
| `--tracking-normal` | 0em |
| `--tracking-wide` | 0.025em |
| `--tracking-wider` | 0.05em |
| `--tracking-widest` | 0.1em |

### Line height (`--leading-*`, unitless)

| Variable | Value |
|---|---|
| `--leading-tight` | 1.25 |
| `--leading-snug` | 1.375 |
| `--leading-normal` | 1.5 |
| `--leading-relaxed` | 1.625 |
| `--leading-loose` | 2 |

### Aspect ratio (`--aspect-*`)

`--aspect-video` = 16 / 9

### Easing (`--ease-*`)

`--ease-in` = cubic-bezier(0.4, 0, 1, 1); `--ease-out` = cubic-bezier(0, 0, 0.2, 1); `--ease-in-out` = cubic-bezier(0.4, 0, 0.2, 1)

### Animations (`--animate-*`)

`--animate-spin`, `--animate-ping`, `--animate-pulse`, `--animate-bounce` — each pairs a duration and timing function with a corresponding `@keyframes` rule.

### Colors (`--color-*`)

The default palette ships 22 named color scales, each with 11 shades (50 through 950), all expressed in OKLCH: red, orange, amber, yellow, lime, green, emerald, teal, cyan, sky, blue, indigo, violet, purple, fuchsia, pink, rose, slate, gray, zinc, neutral, and stone, plus the newer mauve, olive, mist, and taupe scales. Two standalone colors are also defined: `--color-black` (`#000`) and `--color-white` (`#fff`).

### Shadows

The shadow namespaces (`--shadow-*`, `--inset-shadow-*`, `--drop-shadow-*`, `--text-shadow-*`) hold composite multi-part values rather than single dimensions, so they aren't expressed as REM/px conversions.

## Version note

This reference reflects Tailwind CSS v4.3. The four extra color palettes (mauve, olive, mist, taupe) and the `--text-shadow-*` namespace are newer additions in the 4.x line. If you are documenting against a pinned earlier 4.0 release, verify these are present in that specific version before including them.
