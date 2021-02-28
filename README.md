# vite2 + svelte + windicss

## install and start dev
```shell
yarn
yarn dev
yarn build
```

* edit `src/App.svelte`
* remove commments around 'not working' sections and observe

Observations
1) outside @screen is turned into @media
2) nested @apply inside @screen or @media does not work
3) editing replacing @screen with @media while devserver is running causes an error
4) outside scoped class is mysteriously missing from invalid generated @media
```css
@media (min-width: 640px) {
  @apply text-blue-500;
}
h1.svelte-gk50sr {
  --tw-text-opacity: 1;
  color: rgba(255, 62, 0, var(--tw-text-opacity));
  padding: 0.5rem;
  --tw-bg-opacity: 1;
  background-color: rgba(167, 243, 208, var(--tw-bg-opacity));
}
```