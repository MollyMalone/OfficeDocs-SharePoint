---
title: "Manage query spelling correction in SharePoint Server"
ms.author: tlarsen
author: tklarsen
manager: pamgreen
ms.date: 9/8/2017
ms.audience: ITPro
ms.topic: article
ms.prod: sharepoint-server-itpro
localization_priority: Normal
ms.collection: IT_Sharepoint_Server_Top
ms.assetid: eabe099e-5eea-4b33-8241-8079d9409095
description: "Summary: Learn how to include single words in or exclude single words from query spelling corrections to help correct spelling errors in queries."
---

# Manage query spelling correction in SharePoint Server

 **Summary:** Learn how to include single words in or exclude single words from query spelling corrections to help correct spelling errors in queries. 
  
If a user enters a word in a search query that appears to be misspelled, the search results page displays query spelling corrections. This is also known as "Did you mean?". For example, if someone enters a query that contains the word "ampitheater", the query spelling correction would be "amphitheater".
  
These query spelling suggestions are based on the closest matches in the default spelling dictionaries and the Query Spelling Inclusions list. For terms that you enter in the Query Spelling Exclusions list, query spelling suggestions will never be displayed. You can edit the Query Spelling Inclusions and the Query Spelling Exclusions list, but you can't edit the default spelling dictionaries. It takes up to 10 minutes for any changes to the Query Spelling Exclusions or the Query Spelling Inclusions list to take effect.
  
> [!IMPORTANT]
> You can only include or exclude single words. 
  
For more information about linguistic search features for different languages see [Linguistic search features in SharePoint Server](../technical-reference/linguistic-search-features.md).
  
    
## Open the Term Store Management Tool
<a name="QS_OpenTS"> </a>

The query spelling exclusions and inclusions lists are managed in the Term Store. Use the Term Store Management Tool to edit the lists.
  
 **To get to the Term Store Management Tool**
  
1. Verify that the user account that is performing this procedure is an administrator for the Search service application. 
    
2. On the home page of the SharePoint Central Administration website, in the **Application Management** section, click **Manage service applications**.
    
3. On the Manage Service Applications page, click the Search service application.
    
4. On the Search Administration Page, in the **Queries and Results** section, click **Search Dictionaries**. The Term Store Management Tool opens.
    
## Exclude terms from query spelling corrections
<a name="QS_Exclude"> </a>

To exclude words from query spelling corrections, add terms to the Query Spelling Exclusions list.
  
> [!IMPORTANT]
> Create a separate term for each query spelling correction exclusion. Do not create subterms for terms in the Query Spelling Exclusions list. Term hierarchies will be ignored in this context. 
  
 **To add a word to the Query Spelling Exclusions list**
  
1. On the Site Settings: Term Store Management Tool page, click the arrow to expand the **Search Dictionaries** menu. 
    
2. Click Query Spelling Exclusions, click the arrow and then click **Create Term**. 
    
3. Type the word that you want to exclude in the box that appears. 
    
4. Click anywhere on the page to add the term to the Query Spelling Exclusions list.
    
## Include terms in query spelling corrections
<a name="QS_Include"> </a>

To include words in query spelling corrections, add terms to the Query Spelling Inclusions list.
  
> [!IMPORTANT]
> Create a separate term for each query spelling correction inclusion. Do not create subterms for terms in the Query Spelling Inclusions list. Term hierarchies will be ignored in this context. 
  
 **To add a word to the Query Spelling Inclusions list**
  
1. On the Site Settings: Term Store Management Tool page, click the arrow to expand the **Search Dictionaries** menu. 
    
2. Click Query Spelling Inclusions, click the arrow and then click **Create Term**. 
    
3. Type the word that you want to include in the box that appears. 
    
4. Click anywhere on the page to add the term to the Query Spelling Inclusions list.
    
## Edit terms
<a name="QS_Edit"> </a>

You can edit the names of terms in the Query Spelling Exclusions and Query Spelling Inclusions lists. 
  
 **To edit terms**
  
1. On the Site Settings: Term Store Management Tool page, click the arrow to expand the **Search Dictionaries** menu. 
    
2. Depending on which list the term is in, click either **Query Spelling Exclusions** or **Query Spelling Inclusions**.
    
3. Double-click the term that you want to edit. 
    
4. Type the new name for the term.
    
5. Click anywhere on the page to save the edited term.
    
## See also
<a name="QS_Edit"> </a>

[Linguistic search features in SharePoint Server](../technical-reference/linguistic-search-features.md)

[Set-SPEnterpriseSearchQuerySpellingCorrection](http://technet.microsoft.com/library/0c0d069e-d7a8-4341-901a-922188a17705.aspx)
  
[Get-SPEnterpriseSearchQuerySpellingCorrection](http://technet.microsoft.com/library/4a00b085-917b-48c2-a2cc-8252410b2a24.aspx)

