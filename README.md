# LF Edge Foundation Landscape

![LF Edge Landscape Logo](https://raw.githubusercontent.com/State-of-the-Edge/lfedge-landscape/refs/heads/landscapecleanup/images/left-logo.svg)

This landscape is intended as a map to living document that developers, investors, vendors, researchers and others can use as a resource on the landscape of edge computing, a tool to explore open source projects hosted by the LF Edge Foundation, and also shows the LF Edge Foundation member companies. It is modeled after the Cloud Native Computing Foundation (CNCF) [landscape](https://landscape.cncf.io) and based on the same open-source code.

This repository contains the data files and images required to generate the [LF Edge Foundation landscape](https://landscape.lfedge.org). The software that generates it can be found at the [cncf/landscape2](https://github.com/cncf/landscape2) repository. Please see its [README file](https://github.com/cncf/landscape2#landscape2) for more information about how it works.

## New Entries

The requirements for adding new entries for open source projects in the visual and special effects industries is as follows:

* Projects must be open source and hosted on or mirrored to GitHub.
* Edge computing projects with at least 300 GitHub stars that clearly fit in an existing category are generally included. Put the project in the single category where it best fits.
* Projects that clearly fit in an existing category are generally included. Put the project in the single category where it best fits. We are unlikely to create a new category for projects as we'd rather find the best home with the current options.
* Projects a logo and the logo needs to include the name.

If you think your project should be included, please open a pull request to add it to [landscape.yml](landscape.yml). For the logo, upload an SVG to the `hosted_logos` directory.

## Corrections

Please open a pull request with edits to [landscape.yml](landscape.yml).

If the error is with data from [Crunchbase](https://www.crunchbase.com/) you should open an account there and edit the data. If you don't like a project description, edit it in GitHub. If your project isn't showing the license correctly, you may need to paste the unmodified text of the license into a LICENSE file at the root of your project in GitHub, in order for GitHub to serve the license information correctly.

### Updating LF Edge Foundation Members

LF Edge Foundation Member data in this repository ( which in the [landscape.yml](landscape.yml) file is under `LF Edge Member Company` ) are built nightly using the [LFX Landscape Tools](https://github.com/jmertic/lfx-landscape-tools). Any changes made directly in the data files in this repository for LF Edge Foundation Members and Projects will be overwritten.

- For member entries, you can make these changes in [LFX Organization Dashboard](https://docs.linuxfoundation.org/lfx/organization-dashboard/organization-profile).

If you cannot access the above resources, please [create a helpdesk ticket](https://members.lfedge.org) to request those changes.

## Local Build and Install

You can build the landscape locally on your machine using the [landscape2](https://github.com/cncf/landscape2) tool. Once [installed](https://github.com/cncf/landscape2?tab=readme-ov-file#installation), you can use the commands below to build the landscape and serve it locally.

```shell
landscape2 build --data-file landscape.yml --settings-url https://raw.githubusercontent.com/cncf/landscape2-sites/refs/heads/main/lfedge/settings.yml --logos-path hosted_logos --output-dir build
landscape2 serve --landscape-dir build
```

## License

The generated landscape contains data received from [Crunchbase](http://www.crunchbase.com). This data is not licensed pursuant to the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt). It is subject to Crunchbase’s Data Access Terms, available at [https://data.crunchbase.com/docs/terms](https://data.crunchbase.com/docs/terms), and is only permitted to be used with LF Edge Foundation landscape projects.

Everything else is under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt), except for projects and products logos, which are generally copyrighted by the company that created them, and are simply cached here for reliability. The generated landscape and the [landscape.yml](landscape.yml) file are alternatively available under the [Creative Commons Attribution 4.0 license](https://creativecommons.org/licenses/by/4.0/).
