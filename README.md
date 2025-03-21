# ![icon](icons/icon64.png) Piq

Simple cross-platform image browser

![screenshot](icons/screenshot.png)

- Clean UI, no clutter.
- Very fast thumbnail generator (thanks to [sharp#](https://sharp.pixelplumbing.com/)).
- Supports common image files: **jpeg**, **png**, **webp**, **svg**, **gif**, **avif**

## Download

Packages are available for Mac OS and Linux:

[![installer](icons/install.png) Latest Release](https://github.com/slebetman/piq/releases/latest)


# build with docker
/*docker run --rm -ti \
  --env-file <(env | grep -iE 'DEBUG|NODE_|ELECTRON_|YARN_|NPM_|CI|CIRCLE|TRAVIS_TAG|TRAVIS|TRAVIS_REPO_|TRAVIS_BUILD_|TRAVIS_BRANCH|TRAVIS_PULL_REQUEST_|APPVEYOR_|CSC_|GH_|GITHUB_|BT_|AWS_|STRIP|BUILD_') \
  --env ELECTRON_CACHE="/root/.cache/electron" \
  --env ELECTRON_BUILDER_CACHE="/root/.cache/electron-builder" \
  --env SHARP_IGNORE_GLOBAL_LIBVIPS=1 \
  -v ${PWD}:/project \
  -v ~/.cache/electron:/root/.cache/electron \
  -v ~/.cache/electron-builder:/root/.cache/electron-builder \
  electronuserland/builder:wine \
  /bin/bash -c "cd /project && npm install && npx electron-rebuild && npm run build-win"*/