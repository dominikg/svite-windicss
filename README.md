# vite2 + svelte + windicss

## install and start dev
```shell
yarn
yarn dev
```

# edit `src/App.svelte`
remove commments around 'not working' sections and observe

Observations
1) outside @screen is turned into @media
2) nested @apply inside @screen or @media does not work
3) editing replacing @screen with @media while devserver is running causes an error 