# SVoast changelog

## 2.1.2

- Better handling of default options and animations.
- Better comments on types and props.

## 2.1.1

- Fixed default icons being shrunk by max width.

## 2.1.0

- Allowed for string duration timers. To allow for better clarity for those who wish.
  - `1.25s` = `1250`
  - `150ms` = `150`
  - `0.75s` = `750`

## 2.0.0

- Merged `Attention/Check/Cross/Info/Warning.svelte` into a single `Icon.svelte` which receives a `ToastType` and looks up the SVG icon data from a map.

## 1.3.0

- Added `rich` option to allow for rich HTML content in the message.
- Added `onMount` and `onRemove` life cycle hooks.
- `removeById` checks if ID exists in store before removing.

## 1.2.1

- Added `removeAll` method.
- Made `removeById` and `removeByIndex` synchronous.

## 1.2.0

- Added `infinite` prop.
- Renamed `remove` to `removeById` to provide better clairity.
- Added `removeByIndex` which will, remove the toast by the given index.

## 1.1.0

- Rewrite of internal code.
  - This doesn't change anything user side but makes it much easier to maintain.
- `opts` passed prop has been replaced by extracting both options to their own separate prop.
  - `export let opts`, `opts.duration` > `export let duration`, `duration`.
- The `component` option is no longer passed to the toast component.

## 1.0.0

- Allowed the use of custom components.
  - Read the [Docs](https://svoast.vercel.app/#custom-components) to learn more.

## 0.1.1

- Exported all used icons.

## 0.1.0

- Added icon to match the type of toast.
- Fixed smaller toasts stretching to the the width of larger toasts.

## 0.0.1

- Hmmmm toast....
