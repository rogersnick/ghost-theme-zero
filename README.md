# Theme Zero

**Branching off from: https://bulletin.ghost.io**

## Instructions

1. npm run zip to generate a zip file
2. Log into Ghost, and go to the `Design` settings area to upload the zip file

## Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Npm](https://npmjs.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
npm i

# Run build & watch for changes
npm run dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/bulletin.zip`, which you can then upload to your site.

```bash
yarn zip
```

## Running locally with ghost

- Install ghost cli


```bash
npm install ghost-cli@latest -g
```

Then create an empty directory and run the following in it:

```bash
ghost install local
```

The server will automatically start. You can upload a generated zip to see your changes. Use the following commands to control that server:

- `ghost stop` to stop Ghost
- `ghost start` to start Ghost
- `ghost log` views logs
- `ghost ls` to list all running Ghost blogs
- `ghost help` for help

## Copyright & License

Copyright (c) 2013-2023 Ghost Foundation - Released under the [MIT license](LICENSE).
