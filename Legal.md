# Legal Stuff

## Table of Contents

* Introduction
* Copyright
* Licenses
* Applying the Licenses & Copyright
* Contributor License Agreement
* Sanitizing your project
* The NOTICES file
* Terms of Service
* Privacy Statement

## Introduction

Some of the most confusing, complex, and intimidating steps of open sourcing a project have to do with the legal issues surrounding it. Not only is there an abundance of licenses from which to choose, there's also the matter of applying the license once you pick it. And let's not forget copyright. Without copyright over the work, a license doesn't really do much good. So how do you handle not only the initial copyright but also that of any contributors?

Thankfully, the Tagged legal team has already sorted out the answers to these very sticky questions. This makes open sourcing your project a simple matter of following some steps rather than wrestling with legal theories.

## Copyright

According to the [U.S. Copyright Office](http://www.copyright.gov/help/faq/definitions.html), "copyright" is defined as:

> A form of protection provided by the laws of the United States for "original works of authorship", including literary, dramatic, musical, architectural, cartographic, choreographic, pantomimic, pictorial, graphic, sculptural, and audiovisual creations. "Copyright" literally means the right to copy but has come to mean that body of exclusive rights granted by law to copyright owners for protection of their work. Copyright protection does not extend to any idea, procedure, process, system, title, principle, or discovery. Similarly, names, titles, short phrases, slogans, familiar symbols, mere variations of typographic ornamentation, lettering, coloring, and listings of contents or ingredients are not subject to copyright.

Restated and Over-Simplified: The copyright belongs to the creator of a work. It denotes which individual or organization controls or owns the intellectual property of the work.

The copyright for all code, documentation, illustrations, or other works associated with your project and developed by you for Tagged belongs to Tagged. This allows Tagged, if necessary, to protect its intellectual property interests. It also allows Tagged to perform necessary administrative operations on the works. For instance, if Tagged were to create a foundation for supporting and administering all of the open source projects developed and released by Tagged, it would be able to reassign and relinquish control of the copyright to the newly formed foundation. It would not be able to do this if it did not clearly hold the copyright for these projects (you cannot give away what you do not have).

Therefore it is very important that the copyright for each file and work in a project be clearly, explicitly, and properly declared as belonging to Tagged.

## Licenses

A license grants the right for an individual or organization to use (and–in the case of open source projects–copy, modify, or distribute) a copyrighted work and sets forth the conditions and limitations of that use.

Therefore both are necessary when opening your source code or work. A license without a clear copyright is a no-op, since the license would be granting the rights of use based on something which is not defined. Think of it as the legal equivalent of a [NullPointerException](http://docs.oracle.com/javase/7/docs/api/java/lang/NullPointerException.html).

Literally [dozens of open source licenses exist](http://opensource.org/licenses). They all have their advantages and disadvantages, based upon your needs. Thankfully, you don't have to do the work of reviewing every license and weighing them against the needs of the organization. The Tagged legal team has already done this for you.

All code open sourced by Tagged and its employees **must** be released under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html). This license has been chosen not only because of its permissive and community-focused conditions of use, but also because of its thoughtful intellectual property protections.

All documentation, images, and other works open sourced by Tagged and its employees **must** be released under the [Creative Commons Attribution Share Alike License, Version 4.0](https://creativecommons.org/licenses/by-sa/4.0/legalcode).

Please **do not** open source your project under different licenses. The Tagged legal team has approved the Apache v2.0 and CC-BY-SA 4.0 licenses for use and no others.

## Applying the Licenses & Copyright to your project

To make it easier to add the correct license and copyright to your project, we've collected some template files together in a directory which we're calling the [Starter Box](./starter_box).

There are only three steps needed to apply copyright and license properly in your project:

1. Copy the appropriate license file from one of the starter boxes. If your project contains only source code, no documentation, use the [LICENSE-code](./starter_box/LICENSE-code) template. If (like this project), it contains only documentation and not code, use the [LICENSE-docs](./starter_box/LICENSE-docs) template. However, most projects will contain both source code and documentation. Therefore most projects should use the [LICENSE-both](./starter_box/LICENSE-code) template. If you have any doubts about which one to use, just default to using `LICENSE-both`. Whichever license template you use, edit it to replace `[PROJECT]` with the name of the project you are open sourcing.
1. Copy the contents of [copyright_and_license_blurb-code.txt](./starter_box/copyright_and_license_blurb-code.txt). Insert this text at the top of **all** source code files. Yes, each and every source code file. No, there are no exceptions. This text should be placed directly after the [shebang line](http://en.wikipedia.org/wiki/Shebang_(Unix)) (or equivalent) in your source code files.
1. Copy the contents of [copyright_and_license_blurb-docs.txt](./starter_box/copyright_and_license_blurb-docs.txt). Insert this text at the bottom of **all** documentation files, for each file replacing `[FILENAME]` in the blurb with the name of the file being copyrighted and licensed. Yes, each and every doc file. No, there are no exceptions. Yes, we are repeating ourselves. Yes, it's that important.

Voila! You have now applied the copyright and license statements to your project.

## Contributor License Agreement

While the copyright for all work performed by Tagged employees on behalf of Tagged belongs to Tagged itself, the copyright for all work performed by external contributors belongs to each contributor. This is well and proper and the right way of things, but it can cause some administrative headaches.

For instance, what if Tagged actually _were_ to create a non-profit foundation for supporting and administering all of its open source projects? In order to reassign these projects to the purview of the foundation, Tagged would need to receive approval from each and every copyright holder for each and every project. As each contributor holds copyright over their own work, this could mean dozens or even hundreds of copyright holders…for **each** project. Considering how often people move around, change email addresses, or otherwise go AWOL, tracking them all down in order to get their approval to transfer the project to the foundation would be a logistical and administrative nightmare.

Enter the [Contributor License Agreement](./starter_box/CLA.md) (aka the CLA).

A CLA is just a specialized form of license. Just as the Apache License grants the right to use copyrighted software, a CLA is a license which grants the right for an individual or organization to use the work of the contributor. The contributor retains copyright over the work, but Tagged is allowed to distribute and administer the work as needed.

**NOTA BENE**
> Because of the potential legal and administrative snags involved, it is **absolutely vital** that all external contributors to your project have a signed CLA on file **before** you merge their contribution into the project.

So, how do you do that?

### The Contributor License Agreement Process

The process itself is quite simple:

1. Contributor sends in a pull request.
1. You ask the contributor to send in a [signed CLA](./starter_box/CLA_Process.md).
1. Tagged Legal files away the signed CLA then lets you know it's been received.
1. You merge the pull request (after reviewing and approving it, naturally).

However, this assumes that you have provided your contributors with the CLA steps and documents. That's why we've added them to the [Starter Box](./starter_box). Just copy these `CLA*` files to your project and you'll be ready to start accepting contributions from people outside of Tagged.

## Sanitizing your project

Covering your legal bases doesn't end with adding license and copyright statements to your project. You also have to make sure not only that you comply with the copyright and license statements in code on which your code depends, but also that your code doesn't include anything offensive or potentially damaging to Tagged.

### Complying with Others' Copyright and Licensing

If your project imports, uses, or otherwise relies upon code which you and your team did not write, before you open source your project you need to verify that you are using it according to its license. As well, you should acknowledge your debt and gratitude to these projects. That's not a legal thing; it's just good open source citizenship.

To confirm that you are in compliance with the licensing of external code used in your project:

1. Create a list of every piece of external code on which your project relies. It can be an imported library, a piece of cut/pasted code, a published algorithm, or any such resource.
1. For each item on the list, locate the license. If there is no license published, try to contact the author to determine the licensing for the work.
1. Review each license to confirm that your project is in compliance with its strictures. If your project violates the license in any way, these violations **must** be corrected or removed prior to open sourcing the project. If you have any questions about whether your project conforms to the license obligations, immediately contact the Tagged legal team. Don't try to make a "best guess" about legal matters. You leave that to the Legal Team and they'll leave programming to you.
1. Once you've confirmed that your project is in compliance with the licensing restrictions of an external resource, please be a good citizen and acknowledge this resource by listing it in the NOTICES file (see below).

Depending upon the number of external resources on which your project relies, it may take a fair chunk of time to perform this compliance check. Please don't give in to the urge to cut corners here. Just as you'd like people to use your project as you've set forth in your license, please afford others this same courtesy.

### Cleaning up

We are, every one of us, human. As such, our works often have a certain…color to them. Typically born of frustration or amusement, these splashes of color aren't intended to offend. Yet, when viewed by people who are not a part of your team or culture, it's possible that offense may happen (however unintentional).

As well, in our haste to just "get 'er done" we may inadvertently expose sensitive information such as passwords or similarly protected things.

Therefore, before releasing your code as open source, it is absolutely critical that you perform various scans to make sure it's both highly spic and and also very span:

* [Grep](http://en.wikipedia.org/wiki/Grep)/[ack](http://beyondgrep.com/) for all obscenities or variations on obscenities.
* Perform searches for copyrighted or trademarked names or phrases (Google, Facebook, Microsoft, etc.) and remove any which are of questionable value.
* Confirm that **no authorization credentials** are present in the code, configuration, unit tests, or elsewhere in the project.
* Check for "TODO", "XXX", "FIXME" or similar comments in the code. If particularly embarassing, please just fix the problem. If just normal levels of embarassing (we all understand these things, it's OK), let them go but make sure to log them as GitHub Issues once the project is released as open source. An issue unlogged is an issue unfixed.

These searches should be performed not only on the code but also on the commit history for that code. It's not going to do anyone any good to clean up the authorizations in a config file if you're just going to expose them in the commit logs.

## The NOTICES File

The `NOTICES` file is a tricky thing to describe, but may be summarized as "Credit where credit is due."



## Terms of Service

## Privacy Statement

-----

Legal.md: Copyright 2014 Tagged, Inc.

Legal.md is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

You should have received a copy of the license along with this work. If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
