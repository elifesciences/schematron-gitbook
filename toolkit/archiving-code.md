# Archiving code

## Overview

Any code that has been specifically written as part of the work reported in an eLife paper should be made freely accessible under an open-source license. This allows readers to replicate the results using the same tools the authors used. As authors may continue to develop their code in the future, eLife archives the version that exists at the point of publication at [**Software Heritage**](https://www.softwareheritage.org/). Only code that has been created for the specific work should be archived.

It is usually possible to work out whether a repository needs to be archived based on the context:

* Code mentioned in the Data Availability Statement \(e.g. “All analysis code has been made available on GitHub \([**https://github.com/learning-memory-and-decision-lab/NassarBrucknerFrank\_eLife\_2019**](https://github.com/learning-memory-and-decision-lab/NassarBrucknerFrank_eLife_2019)\).”\) should usually be archived.
* If one of the authors of the paper also authored the code, this usually indicates that it was generated for the work and should be archived.
* Code that is mentioned in the text only and referred to as being a ‘package’ is unlikely to have been created for this specific work and therefore doesn’t need to be archived \(unless it is a custom package\). Adding a [**software reference**](../article-details/content/references/software-references.md#how-to-add-a-software-reference) would be more appropriate in these cases. See [**below**](forking-git-based-repos.md#examples-of-code-that-doesnt-need-to-be-forked) for examples of this.
* Any references to custom code or software usually indicates it needs to be archived. 
* If the repository is years old, this usually indicates that the code should not be archived as it probably was not created specifically for the paper.
* Code described in Tools and Resources articles usually does not need to be archived as there will be no results to replicate using it. However, there are some cases where this will be required \([**see below**](archiving-code.md#when-to-fork-code-in-tools-and-resources-papers)\). 

## Checklist for archiving repositories

1. \*\*\*\*[**Check that the repo contains files and is public**](archiving-code.md#check-whether-the-code-is-present-and-public)**.**
2. \*\*\*\*[**Check whether the correct version of the code already exists at Software Heritage**](archiving-code.md#check-whether-the-correct-version-of-the-code-already-exists-at-software-heritage)**.**
3. If it does not, [**archive code at Software Heritage**](archiving-code.md#how-to-archive-code-in-software-heritage)**.**
4. \*\*\*\*[**Add the SWHID to the article text to indicate where the copy is archived**](archiving-code.md#add-the-swhid-to-the-article-text)\*\*\*\*
5. \*\*\*\*[**Add a software reference for the repository**](../article-details/content/references/software-references.md#how-to-add-a-software-reference)\*\*\*\*
6. **Add an author query to indicate the repo has been archived, text updated, and \(if appropriate\) ask the authors to add a license/readme.**

## Check whether the repo contains code and is public

Visit the URL provided in the text. If you see a 404 page such as this:

![](../.gitbook/assets/screenshot-2020-10-06-at-12.12.22.png)

First determine whether there's a typo in the URL. If there's no typo and you cannot determine the correct repo, then add the following author query:

* Please ensure that all scripts/data/code \(as necessary\) are added to this repository, and that it is publicly available. We would also like to ask you to license the contents of the repo \(we would recommend using an open source license \[https://opensource.org/licenses\]\). Guidance on what license might better suit you can be found at https://choosealicense.com/ and instructions on how to add a license to a GitHub repository are available here https://help.github.com/articles/adding-a-license-to-a-repository/. Once your code has been committed and licensed, we will fork it to our own GitHub repository for archiving purposes.

The same action should be taken if the repo is empty

![](https://gblobscdn.gitbook.com/assets%2F-M-TtTNzy5JVpg-oCz26%2F-M8KXAlxtmWpHHSLxNBr%2F-M8KZbLMAnidrlWJhMXW%2FScreen%20Shot%202020-05-26%20at%2011.31.16.png?alt=media&token=9706b81f-4d00-45d6-8338-bf183bb138b2)

All the other steps will have to wait until the authors have responded and acted upon this query.

## Check whether the correct version of the code already exists at Software Heritage

If the repo contains code and is public, go to the [**Software Heritage archive**](https://archive.softwareheritage.org/)**:**

![](../.gitbook/assets/screenshot-2020-10-06-at-11.30.09.png)

Untick 'only show origins visited at least once' and 'filter out origins with no archived content', and enter the URL for the repo containing the code. If it's already archived it will appear in the results.

Check that the result is the correct repo and the most up-to-date version of that repo \(by comparing the latest commit date\). If the code is not the latest version, follow the steps [**below for archiving code**](https://app.gitbook.com/@elifesciences/s/productionhowto/~/drafts/-MIxO7WNOziUlsqSYqlV/toolkit/archiving-code#how-to-archive-code-in-software-heritage).

Here's an example which does _not_ have the most up-to-date version:

![Latest version in SH from January 2020](../.gitbook/assets/screenshot-2020-10-06-at-11.41.25.png)

If there are now results, this indicates that the code has yet to be archived. Follow the steps [**below**](archiving-code.md#how-to-archive-code-in-software-heritage) to do so.

## How to archive code in Software Heritage

From the [**search page**](https://archive.softwareheritage.org/)**,** click 'Save code now' in the left hand panel:

![](../.gitbook/assets/screenshot-2020-10-06-at-11.55.44.png)

This can also be done if looking at a particular repo in Software Heritage:

![](../.gitbook/assets/screenshot-2020-10-06-at-11.44.13%20%281%29.png)

### If the code is in GitHub or GitLab

* Visit the [**save code now page**](https://archive.softwareheritage.org/save/).
* ensure the origin type is 'git' and enter the URL in the 'origin url' field

![](../.gitbook/assets/screenshot-2020-10-06-at-11.47.18.png)

* Click Submit. You should see a green message pop-up:

![](../.gitbook/assets/screenshot-2020-10-06-at-11.47.13.png)

* The status of the archiving can be seen in the 'Browse save requests' tab:

![](../.gitbook/assets/screenshot-2020-10-06-at-11.50.52.png)

The time this process takes is dependent on the contents of the repo, but on average for new repos it may take around 2 hours. Updating repos should be much quicker \(although again this is dependent on the nature of the update\).

### If the code is not in GitHub or GitLab

If the code is stored elsewhere, then you will need to determine what revision control system is used. Bitbucket, Assembla, and SourceFourge all offer other version control in addition to Git, so this will have to be determined from the repo itself.

Any code with git-based revision control systems can follow [**the workflow above**](archiving-code.md#if-the-code-is-in-github-or-gitlab).

Any code with mercurial-based revision control systems can follow [**the workflow above**](archiving-code.md#if-the-code-is-in-github-or-gitlab), but with the caveat that 'hg' instead of 'git' is selected as the Origin type.

Any code with subversion-based revision control systems can follow [**the workflow above**](archiving-code.md#if-the-code-is-in-github-or-gitlab), but with the caveat that 'svn' instead of 'git' is selected as the Origin type.

Any code that does not use git, will need to be deposited. TO BE FLESHED OUT

## **Add the SWHID to the article text**

Software Heritage Identifiers \(SWHID\) are unique and persistent ids used to reference code. They can reference a specific line of code, file, repo, and version of code. For our purposes we want to point to a specific version of a whole repo \(or repos\).

To get a SWHID for a repo, click the 'Permalinks' sidebar tab:

![](../.gitbook/assets/screenshot-2020-10-06-at-12.39.49.png)

Click the revision tab in the sidebar, and **untick** 'Add contextual information':

![](../.gitbook/assets/screenshot-2020-10-06-at-12.41.56.png)

We want to add the abbreviated SWHID to the text with an embedded link to the archived version.

### Add the SWHID to the appropriate place in the text

The authors may have referred to their code in the article text and/or in the data availability statement. 

* If a link to a repository is included the data availability statement, always add the text 'copy archived at XXXXXX', replacing 'XXXXXX' with the SWHID containing the embedded hyperlink.
* If it is included in the article text, you only need to add this text the first time it is mentioned \(note, this needs to be done for each separate repository link if there are multiple\). The authors may only have included this link in their Key Resources Table so make sure the new link is added there if this is the case.

  If the authors have only referred to the code in the data availability statement, add the following query:

  * Please add a mention of your code to the main text of your article so we can add it to your reference list.

* A software reference also needs to be added in the main article \(see [**here**](../article-details/content/references/software-references.md) for how to do this\) - this should only be done after the code has been archived. Please note software citations can't be added in the data availability statement.

#### Example

> Our spike sorting code is freely available at [https://github.com/narendramukherjee/blech\_clust](https://github.com/narendramukherjee/blech_clust) \([Mukherjee, 2019](https://elifesciences.org/articles/45968#bib60); copy archived at [swh:1:rev:86d380144b3f85c8951923de873893583bd25edf](https://archive.softwareheritage.org/swh:1:rev:86d380144b3f85c8951923de873893583bd25edf/)\).

## How to determine whether a repo has an open-source license

For GitHub repositories, the licensing information, if available, can be seen in the 'About section' \(see below\). If this icon is not present, double-check the repository for a file with 'LICENSE' in the name or check the 'README' file which may include licensing information.

![](../.gitbook/assets/screenshot-2020-06-24-at-11.15.54.png)

You can check whether a license is open-source by clicking on it. In the above example, clicking on the MIT license brings up this information: 

![](../.gitbook/assets/screenshot-2020-04-21-at-12.39.19.png)

If the license allows free use, modifications and distribution, it is an open-source license, and the repository can be forked. 

The following are all commonly used open-source licenses:

* \*\*\*\*[**Apache License 2.0**](https://opensource.org/licenses/Apache-2.0)\*\*\*\*
* \*\*\*\*[**BSD 3-Clause "New" or "Revised" license**](https://opensource.org/licenses/BSD-3-Clause)\*\*\*\*
* \*\*\*\*[**BSD 2-Clause "Simplified" or "FreeBSD" license**](https://opensource.org/licenses/BSD-2-Clause)\*\*\*\*
* \*\*\*\*[**GNU General Public License \(GPL\)**](https://opensource.org/licenses/gpl-license)\*\*\*\*
* \*\*\*\*[**GNU Library or "Lesser" General Public License \(LGPL\)**](https://opensource.org/licenses/lgpl-license)\*\*\*\*
* \*\*\*\*[**MIT license**](https://opensource.org/licenses/MIT)\*\*\*\*
* \*\*\*\*[**Mozilla Public License 2.0**](https://opensource.org/licenses/MPL-2.0)\*\*\*\*
* \*\*\*\*[**Common Development and Distribution License**](https://opensource.org/licenses/CDDL-1.0)\*\*\*\*
* \*\*\*\*[**Eclipse Public License version 2.0**](https://opensource.org/licenses/EPL-2.0)\*\*\*\*

## Examples of code that doesn't need to be **archived**

Often, authors will include links or references to software they have used in their studies. These do not need to be archived if they were not generated specifically for the paper. In the example below, none of the GitHub repositories linked need to be archived, as they are references to software that is already available. They should be added as [software references](../article-details/content/references/software-references.md#how-to-add-a-software-reference) instead.

![](../.gitbook/assets/screenshot-2020-04-23-at-10.24.29.png)

## Previously forked or archived repos

Sometimes, authors will refer to code that has been forked or archived for a previous eLife article. While rare, this case occurs most commonly in research advances. No action is required unless the code has been updated since the previous publication. For example, in 55159:

![](../.gitbook/assets/screen-shot-2020-04-24-at-12.35.52.png)

Comparing the forked repositories to the ones that are linked in the article shows that the code has not been updated \(see below, note both repositories were last updated 2 years ago\). Therefore, the repository doesn't need to be forked again. Instead, [software references](../article-details/content/references/software-references.md#how-to-add-a-software-reference) should be added. 

![Repository linked in the article](../.gitbook/assets/screenshot-2020-04-24-at-13.02.03.png)

![Forked repository](../.gitbook/assets/screenshot-2020-04-24-at-13.02.12.png)

The same is true for archived code.

However, if the code has been updated since the fork/archival, then it should be re-archived, and the text should be updated by following the steps from the top of [**the checklist**](archiving-code.md#checklist-for-archiving-repositories).

If someone else’s code has been modified for an eLife paper, this code should not be forked. A [software reference](../article-details/content/references/software-references.md#how-to-add-a-software-reference) to the original code should be added however.

## If a link to a GitHub user is provided

Sometimes authors provide a link to a GitHub user account instead of a specific repository, as in 52658 below:

* All data have been uploaded to https://github.com/horwitzlab.

![](../.gitbook/assets/screenshot-2020-05-27-at-14.19.33.png)

As this does not link to a specific repository, the code cannot be forked. We need the authors to confirm which repository holds the code for the study. Please leave the following author query:

* Please confirm which repositories contain the code for this paper. 

## If code is hosted on an institutional website

Sometimes authors will upload their code to an institutional or lab website. For example, in 54983:

> A comprehensive and curated sequence library was prepared querying the Blastp web server and using a custom Python script \([http://dfns.u-shizuoka-ken.ac.jp/labs/proeng/librarycuration.html](http://dfns.u-shizuoka-ken.ac.jp/labs/proeng/librarycuration.html)\), which exhibited more than 30% sequence identity with E. coli BirA \(EU08004.1\).

The link here is to an institutional website:

![](../.gitbook/assets/screenshot-2020-05-14-at-09.48.43.png)

As it is not possible to fork this, the following query needs to be left:

* We see that you have included a custom script hosted on a lab website. In the interests of transparency and reproducibility, please upload this to a dedicated software repository \(such as GitHub, GitLab etc.\) and ensure that the software is licensed with an open source license \[https://opensource.org/licenses\]. We can provide guidance for you if required. Once your code has been licensed, we will fork it to our own GitHub repository for archiving purposes.

If the link to the code is not to a GitHub/GitLab/SourceForge/Bitbucket repository, and instead to a lab/institution website \(which will usually have the lab's name in the title of the website or on the page\), the above query should be added.

## When to fork code in Tools and Resources papers

If the repository has the same name as the tool being described in the paper, this usually indicates that it should not be forked. For example the data availability statement of 51322 states:

> All data \(schematics, soft- and hardware documentation\) for constructing the MaCaQuE or equivalent systems is made available via GitHub: [https://github.com/sensorimotorgroupdpz/MaCaQuE](https://github.com/sensorimotorgroupdpz/MaCaQuE).

The abstract of this paper states:

> We present an experimental environment \(Reach Cage\) and a versatile visuo-haptic interaction system \(MaCaQuE\) for investigating goal-directed whole-body movements of unrestrained monkeys.

As this paper describing the MaCaQuE system, and the code is for constructing this system, it does not need to be forked.

However, if data was analysed in the paper as in the example below, the linked repositories should be forked. 

![](../.gitbook/assets/screenshot-2020-04-24-at-11.18.10.png)

## If no links or source code files are provided

If authors refer to custom code but there is no link to this and no source code has been provided, please leave the following query:

* We notice that you refer to custom but it seems this hasn't been provided. Please send source code files to production@elifesciences.org, or upload the code to a dedicated software repository \(such as GitHub, GitLab etc.\) and ensure it is licensed with an open source license \[https://opensource.org/licenses\]. Guidance on what license might better suit you can be found at https://choosealicense.com/ and instructions on how to add a license to a GitHub repository are available here https://help.github.com/articles/adding-a-license-to-a-repository/. Once your code has been licensed, we will fork it to our own GitHub repository for archiving purposes.

## Schematron checks

The following tests relate to software that may need to be forked.

#### **code-fork-info**

**Warning**: _Article possibly contains code that needs forking. Search - XXXXXX_

**Action**: This warning will appear if the following words are present: github, gitlab, codeplex, sourceforge, bitbucket or assembla. 'XXXXXX' in this warning will be one of these words. If this warning fires, it may indicate there is code which needs to be forked or imported. [See above](forking-git-based-repos.md#examples-of-code-that-doesnt-need-to-be-forked) to determine whether this is necessary. If the code was specifically written as part of the work reported, it should be forked and a software reference should be added \([**see above**](forking-git-based-repos.md#checklist-for-forking-repositories)\). If it is previously published code please query the author to provide full citation details:

* eLife follows the FAIR principles for software and data citation. Please provide the full bibliographic details \(author\(s\), year, full title, publisher, version, URL\) for this software so that it can be added to the reference list. 

#### ext-link-child-test-3

**Error**: _ext-link - XXXXXX - contains the phrase 'copy archived', which is incorrect._

**Action**: This error will appear if the phrase 'copy archived' is included in the hyperlink to the forked repository. 'XXXXXX' in this error message will be the text which has hyperlink formatting. When pasting in the forked repository link, make sure only the url is hyperlinked. 

## 
