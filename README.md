# Google Maps JavaScript Sample

This sample is generated from @googlemaps/js-samples located at
https://github.com/googlemaps/js-samples.

## Setup

```sh
npm i
npm start  # development
npm run build  # production
```

## Feedback

## Development

### Build

1. `npm i` Install dependencies.
1. `npm run build` Build all targets and update `dist/` folder.

### Test

1. `npm test` Test outputs.
1. (Optional) `npm run lint` Fix lint issues with `npm run format`
1. (Optional) `npm run test:playwright:playground:update-snapshots` Update snapshots. This uses an custom env var to only to only update screenshots that differ from the previous ones (Playwright only supports `none`, `all`, or `missing`). To update all screenshots, use `npm run test:playwright:playground:update-snapshots -- --update-snapshots`. It's possible to target a single sample by using `-g <sample-name>`.

### Run

1. Start a server with all samples using `npm start`

### Staging

For staging samples (not common), use Cloud Source Repositories which are controlled by an access control list.

1. `gcloud auth login`
2. `git config --global credential.https://source.developers.google.com.helper gcloud.sh`
3. `git remote add google https://source.developers.google.com/p/geo-devrel-javascript-samples/r/js-samples`
4. `git push google`
5. `git rev-parse --short HEAD` or visit the [bucket](https://console.cloud.google.com/storage/browser/geo-devrel-javascript-samples-staging).

### Explore

All samples can be explored at https://googlemaps.github.io/js-samples/.

## Other resources

- [Google Maps JavaScript API Documentation](https://developers.google.com/maps/documentation/javascript/tutorial)
- [Google Maps JavaScript API Reference Documentation](https://developers.google.com/maps/documentation/javascript/reference/)
- [Google Maps Typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/google.maps) - `npm i -D @types/google.maps`
- [Google Maps Utilities](https://github.com/googlemaps/v3-utility-library)

## Support

These libraries are community supported. We're comfortable enough with the stability and features of
the libraries that we want you to build real production applications on it.

If you find a bug, or have a feature suggestion, please [log an issue](issues). If you'd like to contribute, please read [How to Contribute](CONTRIB.md).

## add node

docker-compose run --rm -p 30042:8080 node bash
http://localhost:30042

## stop

docker-compose stop

## down

docker-compose down --volumes --remove-orphans
