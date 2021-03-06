# Dependency Analytics

[![Build Status](https://ci.centos.org/job/devtools-fabric8-analytics-vscode-extension/badge/icon)](https://ci.centos.org/job/devtools-fabric8-analytics-vscode-extension/)
[![Chat](https://img.shields.io/badge/chat-on%20mattermost-brightgreen.svg)](https://chat.openshift.io/developers/channels/fabric8-analytics)
[![Visual Studio Marketplace](https://vsmarketplacebadge.apphb.com/version/redhat.fabric8-analytics.svg)](https://marketplace.visualstudio.com/items?itemName=redhat.fabric8-analytics)

'Dependency Analytics Report' with Insights about your application dependencies:
* Flags a security vulnerability(CVE) and suggests a remedial version
* Shows Github popularity metrics along with latest version
* Suggests a project level license, check for conflicts between dependency licences
* AI based guidance for additional, alternative dependencies

## Supported Languages

'Dependency Analytics' extension supports projects using Maven and projects build on npm (Node ecosystem). 
Extending support for Python and Go languages is currently under progress.

## Prerequisites

This extension assumes you have the following binaries on your `PATH`:

* `mvn` (for analyzing Java applications)
* `npm` (for analyzing Node applications)

## Quick Start

  - Install the extension.
  - Opening or editing a manifest file (`pom.xml` / `package.json`) scans your application for security vulnerabilities.
  - Right click on a manifest file (`pom.xml`/`package.json`) in the 'Vscode File explorer' or  'Vscode File editor' to display 'Dependency Analytics Report' for your application.


## Features

1. Opening or editing a manifest file (`pom.xml` / `package.json`) scans your application for security vulnerabilities, flag them along with 'quick fixes'.

![ screencast ](https://raw.githubusercontent.com/fabric8-analytics/fabric8-analytics-vscode-extension/master/images/compAnalysis.gif)

2. Right click on a manifest file(`pom.xml` / `package.json`) and choose 'Dependency Analytics Report ...' to display 'Dependency Analytics' report. This report covers deeper insights into your application dependencies:
* Flags a security vulnerability(CVE) and suggests a remedial version
* Shows Github popularity metrics along with latest version
* Suggests a project level license, check for conflicts between dependency licences
* AI based guidance for additional,alternative dependencies

![ screencast ](https://raw.githubusercontent.com/fabric8-analytics/fabric8-analytics-vscode-extension/master/images/stackanalysis.gif)

3. **For multi module maven application** Right click on root `pom.xml` in editor window and choose 'Dependency Analytics Report ...' to display 'Dependency Analytics' report for the entire application.

![ screencast ](https://raw.githubusercontent.com/fabric8-analytics/fabric8-analytics-vscode-extension/master/images/stackanalysis-multi.gif)

-------------------------------------------------------------------------------------------------------------------
**Note** It creates a folder `target` in workspace which is used for processing of manifest files, needed for generating stack report. So kindly add `target` in `.gitignore`.

Know more about Dependency Analytics Platform
==============================================
The mission of this project is to significantly enhance developer experience:
providing Insights(security, licenses, AI based guidance) for applications and helping developers, Enterprises.

* [GitHub Organization](https://github.com/fabric8-analytics)

Feedback & Questions
====================
* File a bug in [GitHub Issues](https://github.com/fabric8-analytics/fabric8-analytics-vscode-extension/issues)
* Chat with us on [Mattermost](https://chat.openshift.io/developers/channels/fabric8-analytics)

License
=======
Apache 2.0, See [LICENSE](LICENSE) for more information.


