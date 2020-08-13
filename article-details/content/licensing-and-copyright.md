# Licensing and copyright

## Schematron checks

### Content checks

These checks relate to the content of figures and figure supplements. X or XXXXXX refers to quoted text which will change depending on the article.

#### reproduce-test-1

**Warning:** _The caption for XXXXXX contains the text 'reproduced from', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'reproduced from' but there is no permissions information tagged in the XML. If no notes have been left about permissions information to add, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-2

**Warning:** _The caption for XXXXXX contains the text 'reproduced with permission', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'reproduced with permission' but there is no permissions information in the XML. If no notes have been left about permissions information to add, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-3

**Warning:** _The caption for XXXXXX contains the text 'adapted from ...', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'adapted from' but there is no permissions information in the XML. If no notes have been left about permissions information, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-4

**Warning:** _The caption for XXXXXX contains the text 'reprinted from', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'reprinted from' but there is no permissions information in the XML. If no notes have been left about permissions information to add, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-5

**Warning:** _The caption for XXXXXX contains the text 'reprinted with permission', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'reprinted with permission' but there is no permissions information in the XML. If no notes have been left about permissions information, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-6

**Warning:** _The caption for XXXXXX contains the text 'modified from', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'modified from' but there is no permissions information in the XML. If no notes have been left about permissions information, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-7

**Warning:** _The caption for XXXXXX contains the text 'modified with', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'modified with_'_ but there is no permissions information in the XML. If no notes have been left about permissions information, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### reproduce-test-8

**Warning:** _The caption for XXXXXX contains the text 'used with permission', but has no permissions. Is this correct?_

**Action**: This warning will appear if a figure caption includes the text 'used with permission_'_ but there is no permissions information in the XML. If no notes have been left about permissions information, query the Production team who will discuss it with the Editorial team. See more about this [**here**](allowed-assets/figures.md#adapted-and-reproduced-images).

#### fig-permissions-test-1 

**Error:** _permissions for XXXXXX has a copyright-statement, but not a copyright-year or copyright-holder which is incorrect._

**Action**: This will appear if the permissions statement has a copyright statement but no copyright year or holder. These should be added - query the Production team if you don't know what these should be.

#### fig-permissions-test-2

**Error:** _permissions for XXXXXX has a copyright-year, but not a copyright-statement or copyright-holder which is incorrect._

**Action**: This will appear if the permissions statement has a copyright year but no copyright statement or holder. These should be added - query the Production team if you don't know what these should be.

#### fig-permissions-test-3

**Error:** _permissions for XXXXXX has a copyright-holder, but not a copyright-statement or copyright-year which is incorrect._

**Action**: This will appear if the permissions statement has a copyright holder but no copyright statement or year. These should be added - query the Production team if you don't know what these should be.

#### fig-permissions-test-4

**Error:** _permissions for XXXXXX must contain a license-p element._

**Action**: This will appear if the permissions statement doesn't have a &lt;license-p&gt; element. Exeter will need to add this.

#### fig-permissions-test-5

**Error:** _permissions for XXXXXX has XXXXXX &lt;copyright-statement&gt; elements, when there can only be 0 or 1._

**Action**: This will appear if a permissions statement has more than 1 &lt;copyright-statement&gt; element. If the contents of these elements are the same, delete the duplicates. If they are different, double-check what the correct statement should be by comparing with the instructions given by the Production team.

#### fig-permissions-test-6

**Error:** _permissions for XXXXXX has XXXXXX &lt;copyright-holder&gt; elements, when there can only be 0 or 1._

**Action**: This will appear if a permissions statement has more than 1 &lt;copyright-holder&gt; element. If the contents of these elements are the same, delete the duplicates. If they are different, double-check what the correct copyright holder should be by comparing with the instructions given by the Production team.

#### fig-permissions-test-7

**Error:** _permissions for XXXXXX has XXXXXX &lt;copyright-year&gt; elements, when there can only be 0 or 1._

**Action**: This will appear if a permissions statement has more than 1 &lt;copyright-year&gt; element. If the contents of these elements are the same, delete the duplicates. If they are different, double-check what the correct copyright year should be by comparing with the instructions given by the Production team.

#### fig-permissions-test-8

**Error:** _permissions for XXXXXX has XXXXXX &lt;license&gt; elements, when there can only be 0 or 1._ 

**Action**: This error will appear if a permissions statement has more than 1 &lt;license&gt; element. If the contents of these elements are the same, delete the duplicates. If they are different, double-check what the correct license should be by comparing with the instructions given by the Production team.

#### fig-permissions-test-9

**Error**: _permissions for XXXXXX has a &lt;license&gt; element, but not &lt;license-p&gt; element, which is incorrect._

**Action**: This error will appear if a permissions statement has a &lt;license&gt; element but no &lt;license-p&gt; element. Double-check the instructions given by the Production team to see what this should be. 

#### fig-permissions-test-10

**Error**: _permissions for XXXXXX has XXXXXX &lt;license-p&gt; elements, when there can only be 0 or 1._

**Action**: This error will appear if a permissions statement has more than 1 &lt;license-p&gt; element. If the contents of these elements are the same, delete the duplicates. If they are different, double-check what the correct &lt;license-p&gt; text should be by comparing with the instructions given by the Production team.

#### fig-permissions-test-11

**Error**: _figure level permissions must either have a &lt;copyright-statement&gt; or a  &lt;license&gt; element, but those for XXXXXX have neither._

**Action**: This error will appear if a permissions statement has no &lt;copyright-statement&gt; or &lt;license&gt; elements. Query the Production team if these were not provided in the permissions instructions. 

#### fig-permissions-test-12

**Warning**: _XXXXXX permissions - the &lt;license-p&gt; for all rights reserved type permissions should usually end with 'further reproduction of this panel/figure would need permission from the copyright holder.', but XXXXXX's doesn't. Is this correct? \(There is no '_[_https://creativecommons.org/_](https://creativecommons.org/)_' type link so presumed ARR.\)_

**Action**: If the copyright statement for a figure includes 'All rights reserved', the permissions statement should end with 'further reproduction of this panel/figure would need permission from the copyright holder' - you just need to add it in if this is missing. If there is no '[**https://creativecommons.org/**](https://creativecommons.org/)' type link, the schematron will automatically assume the figure permission is 'All rights reserved' - query the Production team to check this is correct. 
