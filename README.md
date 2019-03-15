# CF Sleepy Buildpack

A buildpack that does nothing other than wait a configurable amount of time while staging.

## Configuration

Set the `SLEEPY_TIME` environment variable in your manifest to the number of seconds you want the staging process to sleep.

Note: app files pushed using this buildpack are not served.

Apps with this buildpack as their only or final buildpack serve the text 'OK' on a path of `/`. All other paths serve a 404.

## Example usage

```bash
git clone https://github.com/alphagov/paas-cf-sleepy-buildpack.git
cd cf-sleepy-buildpack/app/
cf push
```
