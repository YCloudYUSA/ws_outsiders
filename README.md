# WS Outsiders Composer Package

## Overview

`ws_outsiders` is a metapackage designed for the YMCA Website Services Drupal distribution. Its primary function is to manage and track Drupal modules and third-party vendor libraries that are not yet fully compatible with the latest major version of Drupal core.

## Purpose

The main goals of this package are:

* **Dependency Management:** To provide a centralized way to include specific versions of modules and libraries that require patches or are pending updates for compatibility with the latest Drupal core.
* **Smooth Upgrades:** To facilitate a smoother upgrade process for the main Drupal distribution by isolating dependencies that need special handling.
* **Tracking "Outsiders":** To maintain a clear record of these "outsider" packages, making it easier to monitor their status and integrate official updates once they become available.

## Usage of `composer replace`

In certain scenarios, this package utilizes the `composer replace` functionality. This allows us to substitute standard package dependencies with custom versions hosted in private Git repositories. This approach is typically employed for:

* **Applying Quick Fixes:** Implementing urgent patches or hotfixes to modules that are critical for the distribution's functionality but have not yet been addressed by the official maintainers.
* **Temporary Forking:** Managing temporary forks of modules where specific modifications are needed to ensure compatibility or to introduce features ahead of official releases.

By using `composer replace`, we can ensure the stability and progress of the YMCA Website Services Drupal distribution while waiting for upstream updates or contributing our fixes back to the community.

## Contributing

Contributions to this metapackage primarily involve updating version constraints, adding new "outsider" packages, or removing packages that have become compatible with the latest Drupal core. Please ensure that any changes are thoroughly tested within the context of the YMCA Website Services Drupal distribution.
