## What 
This is the reproduction for https://github.com/storybookjs/storybook/issues/32028 but also for https://github.com/storybookjs/vite-plugin-storybook-nextjs/issues/79.

## Expected 
`typeof window` logs "object" in the browser console

## Actual 
`typeof window` logs "undefined" in the browser console

## Reproduction steps
1. Clone the code locally `git clone https://github.com/robbchar/next-storybook-typeof-repro`
2. run `yarn install`
3. run `yarn storybook`
4. open the dev tools in your browser
5. click on the Button story
6. notice the output, specifically the line 'typeof window: undefined'

## Versions
Node v22
Next 16.0.7
Storybook 10.1.4
vite 7.2.6
