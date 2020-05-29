---
description: Tabulated content in an article
---

# Tables

Test test 

## Schematron checks

The following tests are run on Tables.

### Content warnings

#### body-table-label-test-1

**Error**: _XXXXXX - Table label does not conform to the usual format._

**Action**: This will fire when a table \(outside of appendices\) has a label which is not in one of the following formats:

* Table 1.
* Key resources table.
* Author response table 1.

Please ensure that the table label is either in one of these formats or \(in the case where it _should not_ have a label\), the label is removed.

#### app-table-label-test-1

**Error**: _XXXXXX - Table label does not conform to the usual format._

**Action**: This will fire when a table in an appendix has a label which is not in the format 'Appendix 1—table 1.' 

Please ensure that there are no typos, missing or extra spaces, that the capitalisation is correct, and that the character between 'Appendix X' and 'table X' is an [em dash](https://www.fileformat.info/info/unicode/char/2014/index.htm).

#### app-table-label-test-2

**Error**: _XXXXXX - Table label does not begin with the title of the appendix it sits in. Either the table is in the incorrect appendix or the table has been labelled incorrectly._

**Action**: This will fire when a table in an appendix has a label which does not start with the title of the appendix that it sties in, for example 'Appendix 1—table 1.' in 'Appendix 2'.

Depending on the case, the table will either need to be moved into its appropriate appendix, or it will need to be re-labelled.

#### table-fn-label-test-1

**Warning**: _Footnote starts with label which is not in line with house style - XXXXXX. Footnote symbols should be in the order: \*, †, ‡, §, ¶, \*\*, ††, ‡‡, §§, ¶¶, etc._

**Action**: This will fire when a table in an appendix has a label which does not start with the title of the appendix that it sties in, for example 'Appendix 1—table 1.' in 'Appendix 2'.

Footnote indicators should be in the follow this sequence _,_ †, ‡, §, ¶, **, ††, ‡‡, §§, ¶¶,** , †††, ‡‡‡, §§§, ¶¶¶, \*\*, ††††, ‡‡‡‡, §§§§, ¶¶¶¶, etc. If this warning fires, it is because a footnote does not start with one of these indicators.

#### distinct-label-conformance

**Error**: _Duplicated labels - XXXXXX is present more than once in the text._

**Action**: This will fire when a Table label occurs twice in the same article. Table labels must be distinct. If this fires, action should be taken to ensure that this label is not used more than once.

#### pre-body-table-report

**Warning**: _XXXXXX_ _does not appear in sequence. Relative to the other numbered tables it is placed in position XX._

**Action**: This will fire when a table is placed out of sequence in the body of an article \(such as Table 1 being placed after Table 2\). If this warning fires, and there is no citation for that table, please add the following author query:

* Please provide an in-text citation for this table.

If there is an in-text citation, but the citations are out of sequence \(i.e. Table 1 being cited after Table 2\), then please add the following author query:

* This citation is out of sequence with the other table citations and has therefore been left unlinked \(table placement is determined by first live citation\). Please confirm this is acceptable.

#### final-body-table-report

**Error**: _XXXXXX_ _does not appear in sequence which is incorrect. Relative to the other numbered tables it is placed in position XX._

**Action**: This will fire when a table is placed out of sequence in the body of an article \(such as Table 1 being placed after Table 2\). If this error fires, Production will need to contact the authors in order to determine how they would like their tables to be labelled/presented.

#### pre-app-table-report

**Warning**: _XXXXXX_ _does not appear in sequence. Relative to the other numbered tables it is placed in position XX._

**Action**: This will fire when a table is placed out of sequence in an appendix \(such as Appendix 1—table 1 being placed after Appendix 1—table 2\). If this warning fires, and there is no citation for that table, please add the following author query:

* Please provide an in-text citation for this table.

If there is an in-text citation, but the citations are out of sequence \(i.e. Appendix 1—table 1 being cited after Appendix 1—table 2\), then please add the following author query:

* This citation is out of sequence with the other table citations and has therefore been left unlinked \(table placement is determined by first live citation\). Please confirm this is acceptable.

#### final-app-table-report

**Error**: _XXXXXX_ _does not appear in sequence which is incorrect. Relative to the other numbered tables it is placed in position XX._

**Action**: This will fire when a table is placed out of sequence in an appendix \(such as Appendix 1—table 1 being placed after Appendix 1—table 2\). If this error fires, Production will need to contact the authors in order to determine how they would like their tables to be labelled/presented.

#### unlinked-object-cite

**Warning**: _XXXXXX has possible unlinked citations in the text._

**Action**: This will fire if a table's label text is found elsewhere in the article without citation formatting \(for example the text 'Table 1' is present in paragraph in the Introduction\). The following actions should be taken:

* If the table citation is deliberately left unlinked due to citations which are out of sequence, this warning can be ignored.
* If the table citation is obviously a reference to a table from another article or piece of work \(e.g. Table 1 from Smith et al., 2020\), then this can be ignored.
* If neither of the above two conditions is the case, then the text should be added as a citation instead.

#### xref-column-test

**Warning**: '_XXXXXX' citation is in a column in the Key Resources Table which usually does not include references. Is it correct?_

**Action**: This will fire if a citation is present in the 1st, 2nd or 4th column in a Key resources table. If it's clear, based on the content of the rest of the table, that the citation should be moved in the 3rd \(headed 'Source/reference'\) or 5th \(headed 'Additional information'\) column, then ensure that it is moved to one of these columns. If it is not clear, and the article is at a pre-author stage, then the following query should be added:

* Please confirm, is this citation in the correct column?

If the article is post-author, then the authors should be queried to check that this is correct \(if they haven't been already\).

#### doi-link-test

**Error**: td element containing - '_XXXXXX_' - looks like it contains a doi, but it contains no link with 'doi.org', which is incorrect.

**Action**: This will fire if a table cell in a Key resources table contains a doi. All dois should be linked in the KR table, so action should be taken to ensure that the doi text has an embedded link \(https://doi.org/{doi}\).

#### PMID-link-test

**Error**: td element containing - 'XXXXXX' - looks like it contains a PMID, but it contains no link pointing to PubMed, which is incorrect.

**Action**: This will fire if a table cell in a Key resources table contains a PMID. All PMIDs should be linked in the KR table, so action should be taken to ensure that the PMID text has an embedded link \(https://www.pubmed.ncbi.nlm.nih.gov/{PMID}\).

#### PMCID-link-test

**Error**: td element containing - 'XXXXXX' - looks like it contains a PMCID, but it contains no link pointing to PMC, which is incorrect.

**Action**: This will fire if a table cell in a Key resources table contains a PMCID. All PMCIDs should be linked in the KR table, so action should be taken to ensure that the PMCID text has an embedded link \(https://www.ncbi.nlm.nih.gov/pmc/{PMCID}\).

#### colour-check-table

**Warning**: XXXXXX element has colour background. Is this correct? It contains XXXXXX.

**Action**: This will fire if a table cell in a table has colour formatting \(a style attribute beginning with 'author-callout'\). eLife only allow the following colours in table cells -  blue, green orange, yellow, purple, red, pink and grey. When this fires an author query should be added to the table \(only 1 per table\):

* Where possible, we prefer that colours are not used in tables in the interests of accessibility. Would it be possible to capture the same meaning in this table with more common forms of emphasis \(such as bold, italic or underline\)? If so please stipulate below how the table should be revised. Please note that this is a suggestion and supported colours in tables can be published.

#### pre-colour-check-table-2

**Warning**: element containing 'XXXXXX' has an @style with an unallowed value - 'XXXXXX'. The only allowed values are 'author-callout-style-b1', 'author-callout-style-b2', 'author-callout-style-b3', 'author-callout-style-b4', 'author-callout-style-b5', 'author-callout-style-b6', 'author-callout-style-b7', 'author-callout-style-b8' for blue, green orange, yellow, purple, red, pink and grey respectively. Please ensure one of these is used. If it is clear that colours are supposed to be used, but you are not sure which ones, then please query the authors - 'eLife only supports the following colours for table cells - blue, green orange, yellow, purple, red, pink and grey. Please confirm how you would like the colour\(s\) here captured given this information.'.

**Action**: This will fire at a pre-author stage if a table cell in a table has a style attribute with an unallowed value. Usually this will be because the colour formatting is not a supported colour. If it _is_ one of the supported colours and this message fires this is a problem - it means that the content has not been typeset correctly.

In the case where it is a colour that is not supported \(brown for example\), then as the message suggests the following author query should be added:

* eLife only supports the following colours for table cells - blue, green orange, yellow, purple, red, pink and grey. Please confirm how you would like the colour\(s\) here captured given this information.

#### final-colour-check-table-2

**Error**: element containing 'XXXXXX' has an @style with an unallowed value - 'XXXXXX'. The only allowed values are 'author-callout-style-b1', 'author-callout-style-b2', 'author-callout-style-b3', 'author-callout-style-b4', 'author-callout-style-b5', 'author-callout-style-b6', 'author-callout-style-b7', 'author-callout-style-b8' for blue, green orange, yellow, purple, red, pink and grey respectively.

**Action**: This will fire at a post-author stage if a table cell in a table has a style attribute with an unallowed value. Usually this will be because the colour formatting is not a supported colour. If it _is_ one of the supported colours and this message fires this is a problem - it means that the content has not been typeset correctly. If it is not a supported colour, ensure to check the author's response to the query which should have been added pre-author. If the response isn't clear about how to proceed \(or the query was mistakenly not left\), then Production will need to contact the author to ask how they would like to proceed.

#### table-wrap-test-3

**Error**: table-wrap has an inline id XXXXX but it has a label - XXXXX, which is not correct.

**Example message**: table-wrap has an inline id inline-table1 but it has a label - Table 1., which is not correct.  

**Action**: This will fire if a table has the incorrect id. A table with a label must have an id in the format `table1`. Either the label needs removing or the table id needs correcting. The original manuscript should be checked to determine which action needs to be taken.

#### table-wrap-test-4

**Error**: table-wrap with id XXXXX has no label which is not correct.

**Action**: This is the inverse of table-wrap-test-3. It will fire if a table without a label has a label which in the format `table1`. Either the label needs adding or the table id needs correcting. The original manuscript should be checked to determine which action needs to be taken.

#### kr-table-wrap-test-1

**Error**: table-wrap has an id XXXXXX but its label is not 'Key resources table', which is incorrect.

**Action**: Key resources tables must have the label 'Key resources table', and an id `keyresource`. This will fire is a table has that id, but it does not have a label, or the label is not exactly as specified above. Action should be taken to ensure both of these conditions are met.

#### pre-table-wrap-cite-1

**Warning**: There is no citation to XXXXXX. Ensure to query the author asking for a citation.

**Action**: This will fire at pre-author stages for tables \(which are not Key resources tables\) with labels, in articles which are not corrections or retractions. If this fires \(and there are no issues with labelling or the table id\), then the following author query should be added:

* Please provide an in-text citation for this table.

The only exception to this is where the article contains an appendix and there is no appropriate place to cite the tables in the appendix \(for example if it is _only_ made up of tables\). In such cases, adding a query is not necessary.

#### final-table-wrap-cite-1

**Warning**: There is no citation to XXXXXX. Ensure this is added.

**Action**: This will fire at post-author stages for tables \(which are not Key resources tables\) with labels, in articles which are not corrections or retractions. If this fires \(and there are no issues with labelling or the table id\), and the authors have not indicated in response to a query where the citation should be, then eLife production should contact the authors to get an appropriate citation.

The only exception to this is where the article contains an appendix and there is no appropriate place to cite the tables in the appendix \(for example if it is _only_ made up of tables\).

#### feat-table-wrap-cite-1

**Warning**: There is no citation to XXXXXX. Is this correct?

**Action**: This will fire at all stages for tables \(which are not Key resources tables\) with labels, in feature content \(insights or feature articles\). 

If this fires at a **pre-author stage** \(and there are no issues with labelling or the table id\), then the following author query should be added:

* Please provide an in-text citation for this table.

If this fires at a **post-author stage**, this should be **ignored** by Exeter and eLife production should check with Features as to whether there should be a citation \(if it isn't already clear\).

#### kr-table-not-tagged

**Error**: XXXXXX has headings that are for the Key resources table, but it does not have an @id='keyresource'.

**Action**: This will at all stages fire if a table has all the KR table headings but does not have an  id `keyresource`. If this fires, ensure that the Table is captured as a Key resources table \(with the correct id, label and no title or caption\).

#### kr-table-not-tagged-2

**Warning**: XXXXXX has the title XXXXXX but it is not tagged as a key resources table. Is this correct?

**Action**: This will fire at all stages if a table has a title containing the text 'Key resource'. If it _is_ a key resources table, then this should be captured as a Key resources table \(with the correct id, label and no title or caption\). If it is not \(i.e. just a normal table, without the standard KR table headings, which happens to have the text 'Key resource' in it's title\), then this message can be ignored.

#### kr-table-header-1

**Warning**: Key resources tables should have 5 column headings \(th elements\) but this one has X. Either it is incorrectly typeset or the author will need to be queried in order to provide the table in the correct format.

**Action**: This will fire at all stages if a KR table does not have the correct number of headings. All KR tables should have 5 headings/columns. If the table is typeset correctly \(**please check this carefully**\), as the author provided it, then the following author query should be added:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-2

**Warning**: Key resources table has more than 1 row in its header, which is incorrect.

**Action**: This will fire at all stages if a KR table has more than one row in it's header. It is **very** likely that this means the table has been incorrectly typeset. If this is the case please correct. If this has been checked very carefully and the table is as the author provided it, then the following author query should be added:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-3

**Warning**: Key resources table has no rows in its header, which is incorrect.

**Action**: This will fire at all stages if a KR table has no rows in it's header. It is **very** likely that this means the table has been incorrectly typeset \(this will almost never occur\). 

#### kr-table-header-4

**Warning**: The first column header in a Key resources table is usually 'Reagent type \(species\) or resource' but this one has 'XXXXXX'.

**Action**: This will fire at all stages if the first header in a KR table is not 'Reagent type \(species\) or resource'. If it's clearly a typo, then this should be corrected. If the table is completely different to how it should be \(see above **LINK TO SECTION**\), then please add the following author query:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-5

**Warning**: The second column header in a Key resources table is usually 'Designation' but this one has 'XXXXXX'.

**Action**: This will fire at all stages if the second header in a KR table is not 'Designation'. If it's clearly a typo, then this should be corrected. If the table is completely different to how it should be \(see above **LINK TO SECTION**\), then please add the following author query:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-6

**Warning**: The third column header in a Key resources table is usually 'Source or reference' but this one has 'XXXXXX'.

**Action**: This will fire at all stages if the third header in a KR table is not 'Source or reference'. If it's clearly a typo, then this should be corrected. If the table is completely different to how it should be \(see above **LINK TO SECTION**\), then please add the following author query:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-7

**Warning**: The fourth column header in a Key resources table is usually 'Identifiers' but this one has 'XXXXXX'.

**Action**: This will fire at all stages if the fourth header in a KR table is not 'Identifiers'. If it's clearly a typo, then this should be corrected. If the table is completely different to how it should be \(see above **LINK TO SECTION**\), then please add the following author query:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### kr-table-header-8

**Warning**: The fifth column header in a Key resources table is usually 'Additional information' but this one has 'XXXXXX'.

**Action**: This will fire at all stages if the fifth header in a KR table is not 'Additional information'. If it's clearly a typo, then this should be corrected. If the table is completely different to how it should be \(see above **LINK TO SECTION**\), then please add the following author query:

* This Key resource table is not in the correct format. Please provide a revised table in the required format using this guide - [https://cdn.elifesciences.org/author-guide/key\_resources\_table.xlsx](https://cdn.elifesciences.org/author-guide/key_resources_table.xlsx). The table can be provided as an editable file \(such as word or excel\) in response to the proofing email. We regret that this was not brought to your attention earlier and apologise for the inconvenience.

#### table-test-2

**Warning**: table doesn't have a header \(thead\). Is this correct?

**Action**: This will fire if a table does not have a header \(the &lt;table&gt; element does not have a child &lt;thead&gt; element\). This could either mean that the table has been incorrectly typeset without headers, or there could be a good reason that it does not have a header \(see **LINK TO SECTION ABOVE**\). If it is an error then this should be fixed by Exeter, otherwise the message can be ignored.

#### tbody-test-1

**Error**: tbody must have at least one row \(tr\).

**Action**: This will fire if the body of a table does not have a row. This is unlikely to occur and if it does, would indicate that the table has been typeset incorrectly, which will need to be fixed by Exeter.

#### thead-test-1

**Error**: thead must have at least one row \(tr\).

**Action**: This will fire if the header of a table does not have a row. This is unlikely to occur and if it does, would indicate that the table has been typeset incorrectly, which will need to be fixed by Exeter.

#### tr-test-1

**Error**: row \(tr\) must contain at least one heading cell \(th\) or data cell \(td\).

**Action**: This will fire if the a row does not have any table cells. This is unlikely to occur and if it does, would indicate that the table has been typeset incorrectly, which will need to be fixed by Exeter.

#### tr-test-2

**Warning**: table row in body contains a th element \(a header\), which is unusual. Please check that this is correct.

**Action**: This will fire for table cells which are styled as headers, but are in the table body. The table has numerous headers throughout it \(and is supposed to\), then this can be ignored. Otherwise Exeter will have to change this to a normal table cell.

#### tr-test-3

**Warning**: table row in body contains a td element \(table data\), which is unusual. Please check that this is correct.

**Action**: This will fire for table cells which are not styled as headers, but are in the header of the table. This is highly unusual, and would usually indicate that either the table should not have a header at all, or that the cell should be given heading formatting.

#### tr-test-3

**Warning**: Table header cell containing 'XXXXXX' has table data \(not header\) cells next to it on the same row. Is this correct? Should the whole row be header cells, or should this cell extend across the whole row?

**Action**: This will fire if a table row contains a mixture of table header cells and normal table cells. This is unusual, although there are a small number of cases where this would be appropriate. Checking the table in the original manuscript will give some indication of how the headings in a table should look like, and if any changes are required these will need to be implemented by Exeter. 

In a case like [this](https://elifesciences.org/articles/53403#table2) 

![](../../.gitbook/assets/screen-shot-2020-05-29-at-12.57.13.png)

all the table cells next to 'Organ' \(in the same row\) should be given table header formatting.

In a case like [this](https://elifesciences.org/articles/52505#table1) 

![](../../.gitbook/assets/screen-shot-2020-05-29-at-12.58.10.png)

'Map resolution' should be made into one cell spanning across its entire row \(formatted as a header\).

In a case like [this](https://elifesciences.org/articles/53498#table1)

![](../../.gitbook/assets/screen-shot-2020-05-29-at-12.54.58.png)

the warning can be ignored, as all the cells in the first column serve as another header.

#### 

### **XML structure warnings**

#### app-table-wrap-id-test-1

**Error**: _table-wrap @id in appendix must be in the format 'app0table0'. XXXXXX does not conform to this._

**Action**: This will fire when the value if the `id` attribute for a table \(with a label\) in the appendix is not in the format `app0table0`. If this fires, it either means that the Table is in the incorrect appendix, or the id needs to be corrected.

#### app-table-wrap-id-test-2

**Error**: _table-wrap @id must start with XXXXXX._

**Action**: This will fire when the value if the `id` attribute for a table \(with a label\) in the appendix does not start with `app` and the appendix number. For example, the ids for any tables in Appendix 1 should start with `app1`. If this fires, it either means that the Table is in the incorrect appendix, or the id needs to be corrected.

#### resp-table-wrap-id-test

**Warning**: _table-wrap @id in author reply must be in the format 'resptable0' or 'sa0table0' if it has a label, or in the format 'respinlinetable0' or 'sa0inlinetable0' if it does not._

**Action**: This will fire when the value if the `id` attribute for a table in the decision letter or author response is not in any of the below formats:

With a label:

* resptable0
* sa0table0

Without a label:

* respinlinetable0
* sa0inlinetable0

Exeter will need to correct this issue if it fires.

#### table-wrap-id-test

**Error**: _table-wrap @id must be in the format 'table0', unless it doesn't have a label, in which case it must be 'inlinetable0' or it is the key resource table which must be 'keyresource'._

**Action**: This will fire when the value if the `id` attribute for a table in the body of an article \(i.e. not in appendices or decision letters or author responses\) is incorrect. If it is a Key resources table, the id must be `keyresource`_._ If the table has a label, it must be in the format `table0`. It it does not have a label, it needs to be in the format `inlinetable0`.

#### table-wrap-test-1

**Error**: table-wrap must have one table.

**Action**: This will fire if a &lt;table-wrap&gt; element does not have a child &lt;table&gt; element. If this fires, it has been typeset incorrectly and steps should be taken to correct it.

#### table-wrap-test-2

**Warning**: table-wrap has more than one table - Is this correct?

**Action**: This will fire if a &lt;table-wrap&gt; element more than one a child &lt;table&gt; element. If the table has two or more sections in it with differing numbers of columns, but it has the same label \(and title\), then this warning can be ignored. If it does not, the table should be collated so that there is only one table element.

#### table-test-1

**Error**: table must have at least one body \(tbody\).

**Action**: This will fire if a &lt;table&gt; element does not have a child &lt;tbody&gt; element. This means that something has gone wrong with the typesetting and the table will need to be corrected.

#### td-child-test

**Error**: td cannot contain XXXXXX. Only the following elements are allowed - 'bold', 'italic', 'sup', 'sub', 'sc', 'ext-link', 'break', 'named-content', 'monospace', and 'xref'.

**Action**: The list of allowed elements correspond to the following types of content respectively - bold, italics, superscript, subscript, small caps, hyperlinks, line breaks, colour formatting, monospace and citations. This will fire if a table data cell contains any other type of content, and will likely need to be corrected by Exeter.

#### th-child-test

**Error**: td cannot contain XXXXXX. Only the following elements are allowed - 'bold', 'italic', 'sup', 'sub', 'sc', 'ext-link', 'break', 'named-content', 'monospace', and 'xref'.

**Action**: The list of allowed elements correspond to the following types of content respectively - bold, italics, superscript, subscript, small caps, hyperlinks, line breaks, colour formatting, monospace and citations. This will fire if a table header cell contains any other type of content, and will likely need to be corrected by Exeter.

#### th-child-test-2

**Warning**: th contains bold. Is this correct?

**Action**: If this fires in live content, then the bold formatting should be removed. Header formatting is always in bold so the bold formatting is superfluous. The only reason this can be ignored is if this fires in an article which is being published as a new version.
