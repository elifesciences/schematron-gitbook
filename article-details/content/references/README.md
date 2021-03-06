---
description: >-
  A guide to reference lists and general rules about references in eLife
  articles
---

# References

## What is a reference list?

Most eLife articles will include a reference list \(otherwise known as a bibliography\) that contains details for all the previous work being cited in the text. These will usually consist mostly of journal articles and books but may also cover websites, papers presented at conferences, software, data and other published material. Whenever research is published, it will be supported with a large number of references; we have had articles with upwards of 150 references. Some review articles, which survey the available literature on a subject, may reach as high as 200+ references.

The reference list is included at the end of the article, in the back matter. References are ordered alphabetically by the surname of the first author for each entry, then by year, and then by the surnames of the second, third, fourth etc authors as necessary. Each reference list covers the entire article in which it appears; references in appendices are not treated separately from those in the main text.

![A typical eLife reference list in the online view](../../../.gitbook/assets/screen-shot-2021-07-13-at-17.06.53.png)

![A reference list in the article PDF](../../../.gitbook/assets/screen-shot-2021-07-13-at-17.07.27.png)

The style used for references in articles - that is, the way the details are formatted and ordered - is derived from the APA style but is unique to eLife. Full author lists are presented online, but where there are more than 20 authors listed, 'et al.' will be used to truncate the list in the PDF \(compare Axten et al., 2021 in the two lists shown above\). This is in order to save space; some journal articles have over 100 authors!

eLife permits references to the following items, for which type-specific guidance has been provided on dedicated pages:

* \*\*\*\*[**Books**](book-references.md)\*\*\*\*
* \*\*\*\*[**Conference papers**](conference-reference.md)\*\*\*\*
* \*\*\*\*[**Data**](data-references.md)\*\*\*\*
* \*\*\*\*[**Journal articles**](journal-references.md)\*\*\*\*
* \*\*\*\*[**Preprints**](preprint-references.md)\*\*\*\*
* \*\*\*\*[**Reports**](report-references.md)\*\*\*\*
* \*\*\*\*[**Software**](software-references.md)\*\*\*\*
* \*\*\*\*[**Theses**](thesis-references.md)\*\*\*\*



## What needs to be checked?



## Schematron warnings

### Content warnings

#### ref-list-title-test

**Warning**: _reference list usually has a title that is 'References', but currently it is 'XXXXXX' - is that correct?_

**Action**:

#### ref-list-distinct-1

**Error**: _In the reference list, each reference must be unique in its citation style \(combination of authors and year\). If a reference's citation is the same as anothers, a lowercase letter should be suffixed to the year \(e.g. Smith et al., 2020a\). XXXXXX does not meet this requirement._

**Action**:

#### err-elem-cit-gen-date-1-2

**Warning**: _The numeric value of the first 4 digits of the &lt;year&gt; element must be between 1700 and the current year + 5 years \(inclusive\). Reference 'XXXXXX' does not meet this requirement as it contains the value 'XXXXXX'._

**Action**:

#### err-elem-cit-gen-date-1-3

**Error**: _All &lt;year&gt; elements must have @iso-8601-date attributes. Reference 'XXXXXX' does not._

**Action**:

#### err-elem-cit-gen-date-1-4

**Warning**: _The numeric value of the first 4 digits of the @iso-8601-date attribute on the &lt;year&gt; element must be between 1700 and the current year + 5 years \(inclusive\). Reference 'XXXXXX' does not meet this requirement as the attribute contains the value 'XXXXXX'._

**Action**:

#### err-elem-cit-gen-date-1-6

**Error**: _If the &lt;year&gt; element contains the letter 'a' after the digits, there must be another reference with the same first author surname \(or collab\) with a letter "b" after the year. Reference 'XXXXXX' does not fulfill this requirement._

**Action**:

#### err-elem-cit-gen-date-1-7

**Error**: _If the &lt;year&gt; element contains any letter other than 'a' after the digits, there must be another reference with the same first author surname \(or collab\) with the preceding letter after the year. Reference 'XXXXXX' does not fulfill this requirement._

**Action:**

#### elem-cit-source

**Error**: _A &lt;source&gt; element within a XXXXXX type &lt;element-citation&gt; must contain at least two characters. - XXXXXX. See Ref 'XXXXXX'._

**Action**:

#### ext-link-attribute-content-match

**Error**: &lt;ext-link&gt; must contain content and have an @xlink:href, the value of which must be the same as the content of &lt;ext-link&gt;. The &lt;ext-link&gt; element in Reference 'XXXXXX' has @xlink:href='XXXXXX' and content 'XXXXXX'.

**Action**:

#### link-href-conformance

**Error**: _@xlink:href must start with either "http://", "https://", or "ftp://". The &lt;ext-link&gt; element in Reference 'XXXXXX' is 'XXXXXX', which does not._

**Action:**

#### err-elem-cit-high-2-2

**Error**: _The order of &lt;element-citation&gt;s in the reference list should be name and date, arranged alphabetically by the first author’s surname, or by the value of the first &lt;collab&gt; element. In the case of two authors, the sequence should be arranged by both authors' surnames, then date. For three or more authors, the sequence should be the first author's surname, then date. Reference 'XXXXXX' appears to be in a different order._

**Action**:

#### err-elem-cit-high-3-3

**Error**: _The sequence of ids in the &lt;ref&gt; elements must increase monotonically \(e.g. 1,2,3,4,5, . . . ,50,51,52,53, . . . etc\). Reference 'XXXXXX' has the value 'XXXXXX', which does not fit this pattern._

**Action**:

#### err-xref-high-2-1

**Error**: _Citations in the text to references with the same author\(s\) in the same year must be arranged in the same order as the reference list. The xref with the value 'XXXXXX' is in the wrong order in the text. Check all the references to citations for the same authors to determine which need to be changed._

**Action**:

#### err-elem-cit-high-6-2

**Error**: _element-citation must have a publication-type attribute with one of these values: 'journal', 'book', 'data', 'patent', 'software', 'preprint', 'web', 'periodical', 'report', 'confproc', or 'thesis'. Reference 'XXXXXX' has 'XXXXXX'._

**Action**:

#### pre-element-cite-year

**Warning**: _'XXXXXX' type references must have a year. Reference 'XXXXXX' does not. If you are unable to determine this, please ensure to add an author query asking for the year of publication._

**Action**:

#### final-element-cite-year

**Error**: _'XXXXXX' type references must have a year. Reference 'XXXXXX' does not. If you are unable to determine this, please ensure to query the authors for the year of publication._

**Action**:

#### pre-element-cite-string-date

**Warning**: '_XXXXXX' type references must have a year. Reference 'XXXXXX' does not. If you are unable to determine this, please ensure to add an author query asking for the year of publication._

**Action**:

#### final-element-cite-string-date

**Error**: _'XXXXXX' type references must have a year. Reference 'XXXXXX' does not. If you are unable to determine this, please ensure to query the authors for the year of publication._

**Action**:

#### pre-pub-id-test-1

**Warning**: _@xlink:href must start with an http:// or ftp:// protocol. - XXXXXX does not. If this information is missing, please ensure to query it with the authors._

**Action**:

#### final-pub-id-test-1

**Error**: _@xlink:href must start with an http:// or ftp:// protocol. - XXXXXX does not._

**Action**:

#### pre-pub-id-test-2

**Warning**: _pub-id is tagged as a doi, but it is not one - XXXXXX. If this information is missing, please ensure to query it with the authors._

**Action**:

#### final-pub-id-test-2

**Error**: _pub-id is tagged as a doi, but it is not one - XXXXXX_

**Action**:

#### pub-id-test-3

**Error**: _pub-id is tagged as a pmid, but it contains a character\(s\) which is not a digit - XXXXXX_

**Action**:

#### pub-id-doi-test-1

**Error**: _pub-id has a doi link - XXXXXX - but its pub-id-type is XXXXXX instead of doi._

**Action**:

#### pub-id-doi-test-2

**Error**: _pub id has a doi link - XXXXXX - but the identifier is not the doi - 'XXXXXX', which is incorrect. Either the doi link is correct, and the identifier needs changing, or the identifier is correct and needs adding after 'https://doi.org/' in order to create the real doi link._

**Action**:

#### pub-id-test-4

**Warning**: _pub id contains whitespace - XXXXXX - which is very likely to be incorrect._

**Action**:

#### pub-id-test-5

**Error**: _XXXXXX pub-id ends with a full stop - XXXXXX - which is not correct. Please remove the full stop._

**Action**:

#### duplicate-ref-test-1

**Error**: _ref 'XXXXXX' has the same doi as another reference, which is incorrect. Is it a duplicate?_

**Action**:

#### duplicate-ref-test-2

**Warning**: _ref 'XXXXXX' has the same doi as another reference, which might be incorrect. If they are not different chapters from the same book, then this is incorrect._

**Action**:

#### duplicate-ref-test-3

**Warning**: _ref 'XXXXXX' has the same title and source as another reference, which is almost certainly incorrect - 'XXXXXX', 'XXXXXX'._

**Action**:

#### duplicate-ref-test-4

**Warning:** _ref 'XXXXXX' has the same title as another reference, but a different source. Is this correct? - 'XXXXXX'_

**Action:** This warning will appear if two references have the same titles. This may happen if the authors include two separate reference lists which have been collated into one, leaving duplicate references. Check the details of both references and if the information is exactly the same, delete one of the duplicates. If the other details of the references differ \(e.g. year, author list, where the article was published\), then both references should be kept. For example, this warning will fire if the two references below are in the same article. However, as the other details of the references differ, both should be kept in the reference list. 

![](../../../.gitbook/assets/screenshot-2020-06-12-at-09.39.00.png)

![](../../../.gitbook/assets/screenshot-2020-06-12-at-09.39.52.png)

#### duplicate-ref-test-6

**Error**: _ref 'XXXXXX' has a doi which is the same as the article itself 'XXXXXX' which must be incorrect._

**Action**:

#### pre-ref-link-presence

**Warning**: _'XXXXXX' has no linked citations. Either the reference should be removed or a citation linking to it needs to be added._

**Action**:

#### final-ref-link-presence

**Error**: _'XXXXXX' has no linked citations. Either the reference should be removed or a citation linking to it needs to be added._

**Action**:

#### ref-given-names-test-1

**Warning**: _Given names should always be initialised. Ref 'XXXXXX' contains a given names with a string longer than 4 characters - 'XXXXXX' in XXXXXX. Is this a surname captured as given names? Or a fully spelt out given names?_

**Action**:





bssubtilis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'B. subtilis' - but there is no italic element with that correct capitalisation or spacing.\_

bacillusssubtilis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Bacillus subtilis' - but there is no italic element with that correct capitalisation or spacing.\_

dsmelanogaster-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'D. melanogaster' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilasmelanogaster-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Drosophila melanogaster' - but there is no italic element with that correct capitalisation or spacing.\_

escoli-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'E. coli' - but there is no italic element with that correct capitalisation or spacing.\_

escherichiascoli-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Escherichia coli' - but there is no italic element with that correct capitalisation or spacing.\_

sspombe-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. pombe' - but there is no italic element with that correct capitalisation or spacing.\_

schizosaccharomycesspombe-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Schizosaccharomyces pombe' - but there is no italic element with that correct capitalisation or spacing.\_

sscerevisiae-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. cerevisiae' - but there is no italic element with that correct capitalisation or spacing.\_

saccharomycesscerevisiae-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Saccharomyces cerevisiae' - but there is no italic element with that correct capitalisation or spacing.\_

cselegans-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'C. elegans' - but there is no italic element with that correct capitalisation or spacing.\_

caenorhabditisselegans-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Caenorhabditis elegans' - but there is no italic element with that correct capitalisation or spacing.\_

asthaliana-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'A. thaliana' - but there is no italic element with that correct capitalisation or spacing.\_

arabidopsissthaliana-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Arabidopsis thaliana' - but there is no italic element with that correct capitalisation or spacing.\_

msthermophila-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'M. thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

myceliophthorasthermophila-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Myceliophthora thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

dictyostelium-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Dictyostelium' - but there is no italic element with that correct capitalisation or spacing.\_

psfalciparum-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'P. falciparum' - but there is no italic element with that correct capitalisation or spacing.\_

plasmodiumsfalciparum-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Plasmodium falciparum' - but there is no italic element with that correct capitalisation or spacing.\_

ssenterica-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. enterica' - but there is no italic element with that correct capitalisation or spacing.\_

salmonellasenterica-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Salmonella enterica' - but there is no italic element with that correct capitalisation or spacing.\_

sspyogenes-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. pyogenes' - but there is no italic element with that correct capitalisation or spacing.\_

streptococcusspyogenes-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Streptococcus pyogenes' - but there is no italic element with that correct capitalisation or spacing.\_

psdumerilii-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'P. dumerilii' - but there is no italic element with that correct capitalisation or spacing.\_

platynereissdumerilii-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Platynereis dumerilii' - but there is no italic element with that correct capitalisation or spacing.\_

pscynocephalus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'P. cynocephalus' - but there is no italic element with that correct capitalisation or spacing.\_

papioscynocephalus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Papio cynocephalus' - but there is no italic element with that correct capitalisation or spacing.\_

osfasciatus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'O. fasciatus' - but there is no italic element with that correct capitalisation or spacing.\_

oncopeltussfasciatus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Oncopeltus fasciatus' - but there is no italic element with that correct capitalisation or spacing.\_

nscrassa-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'N. crassa' - but there is no italic element with that correct capitalisation or spacing.\_

neurosporascrassa-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Neurospora crassa' - but there is no italic element with that correct capitalisation or spacing.\_

csintestinalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'C. intestinalis' - but there is no italic element with that correct capitalisation or spacing.\_

cionasintestinalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Ciona intestinalis' - but there is no italic element with that correct capitalisation or spacing.\_

escuniculi-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'E. cuniculi' - but there is no italic element with that correct capitalisation or spacing.\_

encephalitozoonscuniculi-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Encephalitozoon cuniculi' - but there is no italic element with that correct capitalisation or spacing.\_

hssalinarum-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'H. salinarum' - but there is no italic element with that correct capitalisation or spacing.\_

halobacteriumssalinarum-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Halobacterium salinarum' - but there is no italic element with that correct capitalisation or spacing.\_

sssolfataricus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. solfataricus' - but there is no italic element with that correct capitalisation or spacing.\_

sulfolobusssolfataricus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Sulfolobus solfataricus' - but there is no italic element with that correct capitalisation or spacing.\_

ssmediterranea-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. mediterranea' - but there is no italic element with that correct capitalisation or spacing.\_

schmidteasmediterranea-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Schmidtea mediterranea' - but there is no italic element with that correct capitalisation or spacing.\_

ssrosetta-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. rosetta' - but there is no italic element with that correct capitalisation or spacing.\_

salpingoecasrosetta-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Salpingoeca rosetta' - but there is no italic element with that correct capitalisation or spacing.\_

nsvectensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'N. vectensis' - but there is no italic element with that correct capitalisation or spacing.\_

nematostellasvectensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Nematostella vectensis' - but there is no italic element with that correct capitalisation or spacing.\_

ssaureus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'S. aureus' - but there is no italic element with that correct capitalisation or spacing.\_

staphylococcussaureus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Staphylococcus aureus' - but there is no italic element with that correct capitalisation or spacing.\_

vscholerae-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'V. cholerae' - but there is no italic element with that correct capitalisation or spacing.\_

vibrioscholerae-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Vibrio cholerae' - but there is no italic element with that correct capitalisation or spacing.\_

tsthermophila-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'T. thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

tetrahymenasthermophila-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Tetrahymena thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

csreinhardtii-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'C. reinhardtii' - but there is no italic element with that correct capitalisation or spacing.\_

chlamydomonassreinhardtii-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Chlamydomonas reinhardtii' - but there is no italic element with that correct capitalisation or spacing.\_

nsattenuata-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'N. attenuata' - but there is no italic element with that correct capitalisation or spacing.\_

nicotianasattenuata-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Nicotiana attenuata' - but there is no italic element with that correct capitalisation or spacing.\_

escarotovora-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'E. carotovora' - but there is no italic element with that correct capitalisation or spacing.\_

erwiniascarotovora-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Erwinia carotovora' - but there is no italic element with that correct capitalisation or spacing.\_

esfaecalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'E. faecalis' - but there is no italic element with that correct capitalisation or spacing.\_

hsapiens-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'H. sapiens' - but there is no italic element with that correct capitalisation or spacing.\_

homosapiens-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Homo sapiens' - but there is no italic element with that correct capitalisation or spacing.\_

ctrachomatis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'C. trachomatis' - but there is no italic element with that correct capitalisation or spacing.\_

chlamydiatrachomatis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Chlamydia trachomatis' - but there is no italic element with that correct capitalisation or spacing.\_

enterococcussfaecalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Enterococcus faecalis' - but there is no italic element with that correct capitalisation or spacing.\_

xlaevis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'X. laevis' - but there is no italic element with that correct capitalisation or spacing.\_

xenopuslaevis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Xenopus laevis' - but there is no italic element with that correct capitalisation or spacing.\_

xtropicalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'X. tropicalis' - but there is no italic element with that correct capitalisation or spacing.\_

xenopustropicalis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Xenopus tropicalis' - but there is no italic element with that correct capitalisation or spacing.\_

mmusculus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. musculus' - but there is no italic element with that correct capitalisation or spacing.\_

musmusculus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mus musculus' - but there is no italic element with that correct capitalisation or spacing.\_

dimmigrans-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'D. immigrans' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaimmigrans-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Drosophila immigrans' - but there is no italic element with that correct capitalisation or spacing.\_

dsubobscura-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'D. subobscura' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilasubobscura-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Drosophila subobscura' - but there is no italic element with that correct capitalisation or spacing.\_

daffinis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'D. affinis' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaaffinis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Drosophila affinis' - but there is no italic element with that correct capitalisation or spacing.\_

dobscura-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'D. obscura' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaobscura-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Drosophila obscura' - but there is no italic element with that correct capitalisation or spacing.\_

ftularensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'F. tularensis' - but there is no italic element with that correct capitalisation or spacing.\_

francisellatularensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Francisella tularensis' - but there is no italic element with that correct capitalisation or spacing.\_

pplantaginis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. plantaginis' - but there is no italic element with that correct capitalisation or spacing.\_

podosphaeraplantaginis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Podosphaera plantaginis' - but there is no italic element with that correct capitalisation or spacing.\_

planceolata-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. lanceolata' - but there is no italic element with that correct capitalisation or spacing.\_

plantagolanceolata-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Plantago lanceolata' - but there is no italic element with that correct capitalisation or spacing.\_

mtrossulus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. trossulus' - but there is no italic element with that correct capitalisation or spacing.\_

mytilustrossulus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus trossulus' - but there is no italic element with that correct capitalisation or spacing.\_

medulis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. edulis' - but there is no italic element with that correct capitalisation or spacing.\_

mytilusedulis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus edulis' - but there is no italic element with that correct capitalisation or spacing.\_

mchilensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. chilensis' - but there is no italic element with that correct capitalisation or spacing.\_

mytiluschilensis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus chilensis' - but there is no italic element with that correct capitalisation or spacing.\_

umaydis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'U. maydis' - but there is no italic element with that correct capitalisation or spacing.\_

ustilagomaydis-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Ustilago maydis' - but there is no italic element with that correct capitalisation or spacing.\_

pknowlesi-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. knowlesi' - but there is no italic element with that correct capitalisation or spacing.\_

plasmodiumknowlesi-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Plasmodium knowlesi' - but there is no italic element with that correct capitalisation or spacing.\_

paeruginosa-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. aeruginosa' - but there is no italic element with that correct capitalisation or spacing.\_

pseudomonasaeruginosa-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Pseudomonas aeruginosa' - but there is no italic element with that correct capitalisation or spacing.\_

tbrucei-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'T. brucei' - but there is no italic element with that correct capitalisation or spacing.\_

trypanosomabrucei-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Trypanosoma brucei' - but there is no italic element with that correct capitalisation or spacing.\_

drerio-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'D. rerio' - but there is no italic element with that correct capitalisation or spacing.\_

daniorerio-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_XXXXXX contains an organism - 'Danio rerio' - but there is no italic element with that correct capitalisation or spacing.\_

drosophila-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Drosophila' - but there is no italic element with that correct capitalisation or spacing.\_

xenopus-ref-article-title-check	element-citation/article-title\|element-citation/chapter-title\|element-citation/source\|element-citation/data-title	\*\*Info\*\*: \_ref XXXXXX references an organism - 'Xenopus' - but there is no italic element with that correct capitalisation or spacing.\_

bssubtilis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'B. subtilis' - but there is no italic element with that correct capitalisation or spacing.\_

bacillusssubtilis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Bacillus subtilis' - but there is no italic element with that correct capitalisation or spacing.\_

dsmelanogaster-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. melanogaster' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilasmelanogaster-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila melanogaster' - but there is no italic element with that correct capitalisation or spacing.\_

escoli-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'E. coli' - but there is no italic element with that correct capitalisation or spacing.\_

escherichiascoli-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Escherichia coli' - but there is no italic element with that correct capitalisation or spacing.\_

sspombe-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. pombe' - but there is no italic element with that correct capitalisation or spacing.\_

schizosaccharomycesspombe-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Schizosaccharomyces pombe' - but there is no italic element with that correct capitalisation or spacing.\_

sscerevisiae-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. cerevisiae' - but there is no italic element with that correct capitalisation or spacing.\_

saccharomycesscerevisiae-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Saccharomyces cerevisiae' - but there is no italic element with that correct capitalisation or spacing.\_

cselegans-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'C. elegans' - but there is no italic element with that correct capitalisation or spacing.\_

caenorhabditisselegans-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Caenorhabditis elegans' - but there is no italic element with that correct capitalisation or spacing.\_

asthaliana-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'A. thaliana' - but there is no italic element with that correct capitalisation or spacing.\_

arabidopsissthaliana-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Arabidopsis thaliana' - but there is no italic element with that correct capitalisation or spacing.\_

msthermophila-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'M. thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

myceliophthorasthermophila-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Myceliophthora thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

dictyostelium-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Dictyostelium' - but there is no italic element with that correct capitalisation or spacing.\_

psfalciparum-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'P. falciparum' - but there is no italic element with that correct capitalisation or spacing.\_

plasmodiumsfalciparum-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Plasmodium falciparum' - but there is no italic element with that correct capitalisation or spacing.\_

ssenterica-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. enterica' - but there is no italic element with that correct capitalisation or spacing.\_

salmonellasenterica-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Salmonella enterica' - but there is no italic element with that correct capitalisation or spacing.\_

sspyogenes-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. pyogenes' - but there is no italic element with that correct capitalisation or spacing.\_

streptococcusspyogenes-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Streptococcus pyogenes' - but there is no italic element with that correct capitalisation or spacing.\_

psdumerilii-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'P. dumerilii' - but there is no italic element with that correct capitalisation or spacing.\_

platynereissdumerilii-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Platynereis dumerilii' - but there is no italic element with that correct capitalisation or spacing.\_

pscynocephalus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'P. cynocephalus' - but there is no italic element with that correct capitalisation or spacing.\_

papioscynocephalus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Papio cynocephalus' - but there is no italic element with that correct capitalisation or spacing.\_

osfasciatus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'O. fasciatus' - but there is no italic element with that correct capitalisation or spacing.\_

oncopeltussfasciatus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Oncopeltus fasciatus' - but there is no italic element with that correct capitalisation or spacing.\_

nscrassa-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'N. crassa' - but there is no italic element with that correct capitalisation or spacing.\_

neurosporascrassa-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Neurospora crassa' - but there is no italic element with that correct capitalisation or spacing.\_

csintestinalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'C. intestinalis' - but there is no italic element with that correct capitalisation or spacing.\_

cionasintestinalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Ciona intestinalis' - but there is no italic element with that correct capitalisation or spacing.\_

escuniculi-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'E. cuniculi' - but there is no italic element with that correct capitalisation or spacing.\_

encephalitozoonscuniculi-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Encephalitozoon cuniculi' - but there is no italic element with that correct capitalisation or spacing.\_

hssalinarum-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'H. salinarum' - but there is no italic element with that correct capitalisation or spacing.\_

halobacteriumssalinarum-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Halobacterium salinarum' - but there is no italic element with that correct capitalisation or spacing.\_

sssolfataricus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. solfataricus' - but there is no italic element with that correct capitalisation or spacing.\_

sulfolobusssolfataricus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Sulfolobus solfataricus' - but there is no italic element with that correct capitalisation or spacing.\_

ssmediterranea-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. mediterranea' - but there is no italic element with that correct capitalisation or spacing.\_

schmidteasmediterranea-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Schmidtea mediterranea' - but there is no italic element with that correct capitalisation or spacing.\_

ssrosetta-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. rosetta' - but there is no italic element with that correct capitalisation or spacing.\_

salpingoecasrosetta-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Salpingoeca rosetta' - but there is no italic element with that correct capitalisation or spacing.\_

nsvectensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'N. vectensis' - but there is no italic element with that correct capitalisation or spacing.\_

nematostellasvectensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Nematostella vectensis' - but there is no italic element with that correct capitalisation or spacing.\_

ssaureus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'S. aureus' - but there is no italic element with that correct capitalisation or spacing.\_

staphylococcussaureus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Staphylococcus aureus' - but there is no italic element with that correct capitalisation or spacing.\_

vscholerae-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'V. cholerae' - but there is no italic element with that correct capitalisation or spacing.\_

vibrioscholerae-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Vibrio cholerae' - but there is no italic element with that correct capitalisation or spacing.\_

tsthermophila-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'T. thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

tetrahymenasthermophila-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Tetrahymena thermophila' - but there is no italic element with that correct capitalisation or spacing.\_

csreinhardtii-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'C. reinhardtii' - but there is no italic element with that correct capitalisation or spacing.\_

chlamydomonassreinhardtii-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Chlamydomonas reinhardtii' - but there is no italic element with that correct capitalisation or spacing.\_

nsattenuata-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'N. attenuata' - but there is no italic element with that correct capitalisation or spacing.\_

nicotianasattenuata-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Nicotiana attenuata' - but there is no italic element with that correct capitalisation or spacing.\_

escarotovora-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'E. carotovora' - but there is no italic element with that correct capitalisation or spacing.\_

erwiniascarotovora-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Erwinia carotovora' - but there is no italic element with that correct capitalisation or spacing.\_

hsapiens-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'H. sapiens' - but there is no italic element with that correct capitalisation or spacing.\_

homosapiens-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Homo sapiens' - but there is no italic element with that correct capitalisation or spacing.\_

ctrachomatis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'C. trachomatis' - but there is no italic element with that correct capitalisation or spacing.\_

chlamydiatrachomatis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Chlamydia trachomatis' - but there is no italic element with that correct capitalisation or spacing.\_

esfaecalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'E. faecalis' - but there is no italic element with that correct capitalisation or spacing.\_

enterococcussfaecalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Enterococcus faecalis' - but there is no italic element with that correct capitalisation or spacing.\_

xlaevis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'X. laevis' - but there is no italic element with that correct capitalisation or spacing.\_

xenopuslaevis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Xenopus laevis' - but there is no italic element with that correct capitalisation or spacing.\_

xtropicalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'X. tropicalis' - but there is no italic element with that correct capitalisation or spacing.\_

xenopustropicalis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Xenopus tropicalis' - but there is no italic element with that correct capitalisation or spacing.\_

mmusculus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'M. musculus' - but there is no italic element with that correct capitalisation or spacing.\_

musmusculus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Mus musculus' - but there is no italic element with that correct capitalisation or spacing.\_

dimmigrans-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. immigrans' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaimmigrans-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila immigrans' - but there is no italic element with that correct capitalisation or spacing.\_

dsubobscura-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. subobscura' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilasubobscura-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila subobscura' - but there is no italic element with that correct capitalisation or spacing.\_

daffinis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. affinis' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaaffinis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila affinis' - but there is no italic element with that correct capitalisation or spacing.\_

dobscura-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. obscura' - but there is no italic element with that correct capitalisation or spacing.\_

drosophilaobscura-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila obscura' - but there is no italic element with that correct capitalisation or spacing.\_

ftularensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'F. tularensis' - but there is no italic element with that correct capitalisation or spacing.\_

francisellatularensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Francisella tularensis' - but there is no italic element with that correct capitalisation or spacing.\_

pplantaginis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'P. plantaginis' - but there is no italic element with that correct capitalisation or spacing.\_

podosphaeraplantaginis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Podosphaera plantaginis' - but there is no italic element with that correct capitalisation or spacing.\_

planceolata-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'P. lanceolata' - but there is no italic element with that correct capitalisation or spacing.\_

plantagolanceolata-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Plantago lanceolata' - but there is no italic element with that correct capitalisation or spacing.\_

mtrossulus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. trossulus' - but there is no italic element with that correct capitalisation or spacing.\_

mytilustrossulus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus trossulus' - but there is no italic element with that correct capitalisation or spacing.\_

medulis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. edulis' - but there is no italic element with that correct capitalisation or spacing.\_

mytilusedulis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus edulis' - but there is no italic element with that correct capitalisation or spacing.\_

mchilensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'M. chilensis' - but there is no italic element with that correct capitalisation or spacing.\_

mytiluschilensis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Mytilus chilensis' - but there is no italic element with that correct capitalisation or spacing.\_

umaydis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'U. maydis' - but there is no italic element with that correct capitalisation or spacing.\_

ustilagomaydis-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Ustilago maydis' - but there is no italic element with that correct capitalisation or spacing.\_

pknowlesi-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. knowlesi' - but there is no italic element with that correct capitalisation or spacing.\_

plasmodiumknowlesi-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Plasmodium knowlesi' - but there is no italic element with that correct capitalisation or spacing.\_

paeruginosa-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'P. aeruginosa' - but there is no italic element with that correct capitalisation or spacing.\_

pseudomonasaeruginosa-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Info\*\*: \_XXXXXX contains an organism - 'Pseudomonas aeruginosa' - but there is no italic element with that correct capitalisation or spacing.\_

tbrucei-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'T. brucei' - but there is no italic element with that correct capitalisation or spacing.\_

trypanosomabrucei-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Trypanosoma brucei' - but there is no italic element with that correct capitalisation or spacing.\_

drerio-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'D. rerio' - but there is no italic element with that correct capitalisation or spacing.\_

daniorerio-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Danio rerio' - but there is no italic element with that correct capitalisation or spacing.\_

drosophila-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Drosophila' - but there is no italic element with that correct capitalisation or spacing.\_

xenopus-article-title-check	article//article-meta/title-group/article-title \| article/body//sec/title \| article//article-meta//kwd	\*\*Warning\*\*: \_XXXXXX contains an organism - 'Xenopus' - but there is no italic element with that correct capitalisation or spacing.\_





### XML structure warnings

#### pre-err-elem-cit-gen-date-1-5

**Warning**: _The numeric value of the first 4 digits of the @iso-8601-date attribute must match the first 4 digits on the &lt;year&gt; element. Reference 'XXXXXX' does not meet this requirement as the element contains the value 'XXXXXX' and the attribute contains the value 'XXXXXX'. If there is no year, and you are unable to determine this, please query with the authors._

**Action**:

#### final-err-elem-cit-gen-date-1-5

**Error**: _The numeric value of the first 4 digits of the @iso-8601-date attribute must match the first 4 digits on the &lt;year&gt; element. Reference 'XXXXXX' does not meet this requirement as the element contains the value 'XXXXXX' and the attribute contains the value 'XXXXXX'. If there is no year, and you are unable to determine this, please query with the authors._

**Action**:

#### err-elem-cit-high-1

**Error**: _The only element that is allowed as a child of &lt;ref&gt; is &lt;element-citation&gt;. Reference 'XXXXXX' has other elements._

**Action**:

#### err-elem-cit-high-3-1

**Error**: _Each &lt;ref&gt; element must have an @id attribute._

**Action**: 

#### err-elem-cit-high-3-2

**Error**: _Each &lt;ref&gt; element must have an @id attribute that starts with 'bib' and ends with a number. Reference 'XXXXXX' has the value 'XXXXXX', which is incorrect._

**Action**: 

#### pre-empty-elem-cit-des

**Warning**: _XXXXXX element is empty - this is not allowed. It must contain content. If the details are missing and cannot be determined, please query the authors._

**Action**:

#### final-empty-elem-cit-des

**Error**: _XXXXXX element is empty - this is not allowed. It must contain content._

**Action**:

#### tagging-elem-cit-des

**Error**: _XXXXXX element contains tagging, which should be removed - 'XXXXXX'._

**Action**:

