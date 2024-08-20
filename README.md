# idh-packages
Packages used by IDH team

## chromium
We are currently using Puppeteer 16.2.0, for which the default Chromium version is 105.0.5173.0 (1022525).
Unfortunately Puppeteer does not have arm64 support, so it cannot download the binary itself. So we need
to find compiled binaries for a version as close as possible to the original and use them instead. The
closest ones are from Ubuntu bionic repo, so we are using archive builds from:
* amd64: https://launchpad.net/~canonical-chromium-builds/+archive/ubuntu/stage/+build/24341307
* arm64: https://launchpad.net/~canonical-chromium-builds/+archive/ubuntu/stage/+build/24341308
This version is 105.0.5195.102-0ubuntu0.18.04.1
