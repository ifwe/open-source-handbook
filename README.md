# The Tagged Open Source Handbook

This is the handbook for how to open source your projects at [Tagged](http://tagged.com).

While this document is written for Tagged team members, it is licensed under the [CC-BY-SA](http://creativecommons.org/licenses/by-sa/4.0) license and is free for use by all who wish to release their projects as open source.

## Table of Contents

* [Introduction](#introduction)
* [TL;DR](#tldr)
* [Legal Stuff](./Legal.md)
   * [Copyright](./Legal.md#copyright)
   * [License](./Legal.md#license)
   * [Applying the License & Copyright](./Legal.md#applying-the-licenses--copyright-to-your-project)
   * [Contributor License Agreement](./Legal.md#contributor-license-agreement)
   * [Sanitizing your project](./Legal.md#sanititizing-your-project)
   * [The NOTICES file](./Legal.md#the-notices-file)
   * [Terms of Service](./Legal.md#terms-of-service)
   * [Privacy Statement](./Legal.md#privacy-statement)
* Contributing
   * How to Contribute (aka The CONTRIBUTING file)
   * Submitting code
      * Coding conventions
   * Submitting documentation
      * Style guide
   * The AUTHORS file
* Community
   * Code of Conduct
   * Users
   * Contributors
   * Social Networking
* Documentation
   * The README file
   * User docs
      * Usage examples
   * Developer docs
      * API
      * Code examples
   * FAQ
   * Wiki
   * Project website
* Nuts & Bolts
   * Source Control
   * Issue Tracker
   * Packaging, Distribution, & Installation
   * Versioning
   * Unit Tests
   * Continuous Integration
   * Project Accounts Authorizations & Passwords
* Communication
   * Working with Marcom
* [Contributing to this document](./CONTRIBUTING.md)
* [FAQ](./FAQ.md)
* [Other Resources](./Resources.md)

## Introduction

[Tagged](http://tagged.com) is dedicated to [open
source](http://opensource.org/osd). We believe that we are stronger together than separately and that free and open software and other resources (such as this document) are a rising tide which lifts all boats.

To that end, Tagged tries to open source as many of its internally-developed resources as it can.

However, open sourcing your project is much more than simply dropping your code into a [GitHub repository](http://github.com/tagged) and walking away. There are a lot of legal, procedural, and usability hoops to jump through to open source a project properly. We realize that it can be a daunting task for those who're not familiar with the process. Don't worry: We're here to help.

This document will clarify the process and show you exactly what you need to do not only to release your project as open source, but also to maintain it and its community afterward.

**NOTA BENE**:

> All Tagged projects should use this process. It is standardized in order to make it easier for all current and future team members and to eliminate guesswork. If you need to diverge from the guidelines set forth in this document, please consult with your team lead, manager, and other stakeholders before doing so.

## TL;DR

> Much words. Many readings. Wow.

We realize that this is a long document and that, really, all you want to do is just get your code released and then get back to making great stuff which enables meaningful connections between people. Honest, we get that and we love it about you.

So we've summed up the entire process in a single itemized list. There are still a lot of steps here, but this list should make it easier for you to dot all your i's and cross all your t's without spending too much time slogging through documentation.

That said, we strongly suggest you read this entire document at least once. Afterward you'll understand not only what to do to open source your project, you'll also understand **why**.

Keep in mind: The items on the list below are **not** optional. Please make sure that each step is complete. Don't skip any for any reason. They are all necessary to make sure your project is properly open sourced.

To make it easier to open source your project, we've collected some template files together in the [Starter Box](./starter_box) directory. You can simply copy the necessary files/text from there.

Here are the steps for open sourcing your project:

1. Get approval from your team lead or manager.
1. Notify Marcom that a new project will be open sourced shortly.
1. Review the project to make sure it's not divulging any sensitive information (passwords, etc.).
1. Review the commit history for the project to make sure it's not divulging any sensitive information.
1. If the project uses any external libraries or code, review their licenses to confirm that they are compatible with the Apache v2.0 License.
1. Make sure the project contains the following files:
    * README (in either plain text or Markdown format)
    * LICENSE (containing both the Apache v2.0 and the CC-BY-SA licenses)
    * CONTRIBUTING (in either plain text or Markdown format)
    * Contributor License Agreement and instructions
    * AUTHORS (either in plain text or Markdown format)
    * Code of Conduct
1. Apply the Tagged, Inc. copyright to all files.
1. Apply the Apache v2.0 License to all code.
1. Apply the CC-BY-SA License to all documentation.
1. Make the repository public in the Tagged organization on [GitHub](https://github.com/tagged).
1. Confirm that any internal processes (continuous integration, etc.) now point to the new public repository.
1. End of life the internal (private) repository.
1. Notify Marcom that a new project has been released to the world!

-----

README.md: Copyright 2014 Tagged, Inc.

README.md is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

You should have received a copy of the license along with this work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
