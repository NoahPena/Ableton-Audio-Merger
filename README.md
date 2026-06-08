# Audio Merger

Audio Merger is an Ableton Live Extension that can merge all audio within an Arrangement Audio Selection into a single file on a new Track.

## Limitations

There are a couple limitations due to limitations with the Ableton Extension SDK. Namely:

* Audio Merger only merges Pre-FX Audio since there is no way to render Post-FX Audio
* MIDI Clips are not supported because there is no way to bounce a MIDI Track to an Audio Clip
    * Any MIDI Clips selected are just skipped


## Get Started

Learn about building extensions: https://ableton.github.io/extensions-sdk/

## Setup

The path to Ableton Live's Extension Host module is stored in `.env` as
`EXTENSION_HOST_PATH`. The generator filled this in for you; edit it if your
install moves.

## Scripts

```sh
npm start                  # build + run in Live's Extension Host
npm run build              # production bundle of src/extension.ts
npm run build:dev          # dev bundle (sourcemaps, not minified)
npm run package            # build for production + create a .ablx archive
```
