# CF Sleepy Buildpack

A buildpack that does nothing other than wait a configurable amount of time while staging.

## Configuration

Set the `SLEEPY_TIME` environment variable in your manifest to the number of seconds you want the staging process to sleep.

Note: app files pushed using this buildpack are not served. It only serves the text 'OK' via Netcat.

## Example usage

```bash
git clone https://github.com/henrytk/cf-sleepy-buildpack.git
cd cf-sleepy-buildpack/app/
cf push
```
