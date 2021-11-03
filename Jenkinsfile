/** This is the entirety of the core pipeline file.

It should only be used to trigger code in the [divvy-dev-builder](https://github.com/rapid7/divvy-dev-builder) library,
which is in it's own repository.

The `vars` folder contains the divvyDevBuild entrypoint utilized below.
*/

// Do not delete or move into shared library.
// If this is removed or moved elsewhere, multiple simultaneous builds for a branch can occur.
properties([
        disableConcurrentBuilds()
])

/**
Load and execute the [divvy-dev-builder](https://github.com/rapid7/divvy-dev-builder) library.
*/
@Library('divvy-dev-builder@divvy-new-release') _
divvyDevBuild(this)
