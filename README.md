## Local Setup

1. Add `pnpm` globally via `npm i -g pnpm`
2. Install dependencies by running `pnpm install`
3. Start Storybook with the command `pnpm storybook`

## Repro steps

1. While Storybook is running in the browser (Chrome), navigate to `src/stories/button.css.ts`
2. Make a change to the styles, e.g. change fontSize property to '100px'.

## What happens

HMR kicks in but Storybook can no longer find the component. I have to do a full page reload to get the updated component

## What should happen

HMR kicks in and the component styles gets updated without any issues.
