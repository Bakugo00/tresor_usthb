# Change Log

## [1.1.0] 2021-03-19
### Bug fixing
- Rename `master` branch to `main`
- To make a lot of our changes, we've followed the instructions from here (minus the `colors` and `font-sizes`): https://tailwindcss.com/docs/upgrading-to-v2
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-gray-{number}` classes were renamed to `{type}-blueGray-{number}`
  - After that, we've changed `{type}-blueGray-{number}` to `{type}-blueGray-{lower-number}`, i.e. (`100` became `50`, `200` became `100`, ..., `900` became `800`)
    - You can achieve this, by search in your whole project for `blueGray-100` and replace it with `blueGray-50`
    - Then, you search in your whole project for `blueGray-200` and replace it with `blueGray-100`
    - Then, you search in your whole project for `blueGray-300` and replace it with `blueGray-200`
    - Then, you search in your whole project for `blueGray-400` and replace it with `blueGray-300`
    - Then, you search in your whole project for `blueGray-500` and replace it with `blueGray-400`
    - Then, you search in your whole project for `blueGray-600` and replace it with `blueGray-500`
    - Then, you search in your whole project for `blueGray-700` and replace it with `blueGray-600`
    - Then, you search in your whole project for `blueGray-800` and replace it with `blueGray-700`
    - Then, you search in your whole project for `blueGray-900` and replace it with `blueGray-800`
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-blue-{number}` classes were renamed to `{type}-lightBlue-{number}`
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-green-{number}` classes were renamed to `{type}-emerald-{number}`
- `lg:bg-transparent` is not working anymore, so we've changed it with `lg:bg-opacity-0`

### Deleted dependencies
- `@tailwindcss/custom-forms`
- `react-google-maps` (replaced by simple Google Maps API)
- `@types/googlemaps` (dependencies of `react-google-maps`)
- `@types/markerclustererplus` (dependencies of `react-google-maps`)
- `@types/react` (dependencies of `react-google-maps`)
### Added dependencies
- `@tailwindcss/forms` (replaces `@tailwindcss/custom-forms`)
- `autoprefixer`
- `postcss`
### Updated dependencies
```
@fortawesome/fontawesome-free    5.14.0   →   5.15.3
@popperjs/core                    2.5.1   →    2.9.1
chart.js                          2.9.3   →    2.9.4
react                           16.13.1   →   17.0.1
react-dom                       16.13.1   →   17.0.1
react-scripts                     3.4.3   →    4.0.3
tailwindcss                      1.8.10   →    2.0.4
typescript                        4.0.3   →    4.2.3
```

