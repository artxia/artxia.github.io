---
layout: handbook-page-toc
title: "Searching The GitLab Website like a pro"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Challenge

At GitLab, we're prolific at [documenting what we do in the handbook](/handbook/handbook-usage/#why-handbook-first), the website, and in GitLab [documentation](/company/culture/all-remote/management/#scaling-by-documenting). This may make it difficult to find specific pieces of content.

## Basic solution —  "search site:"

Google already indexes all our public facing pages and there is a [search modifier Google offers that will help](https://support.google.com/websearch/answer/2466433?hl=en).

> **Search for a specific site**<br>
Put "site:" in front of a site or domain. For example, `site:youtube.com`.

If you are looking for information on the GitLab "team", then simply type this into the Google search:<br><br> `team site:about.gitlab.com`

The Google search results will be **only** from `about.gitlab.com`.

Similarly, if you're looking for "permissions" in GitLab product documentation, then simply type this into search: <br><br>`permissions site:docs.gitlab.com`

The Google search results will be **only** be documentation from `docs.gitlab.com`.

This also works for specific subdirectories. For example, if you **only** want to search in the handbook for "values" you can type

`site:about.gitlab.com/handbook/values`

## Advanced solution

The `site:` technique is incredibly powerful. But, if you use it often, you end up typing the URL all the time — not very efficient. If you use Chrome, there is a simple trick to use Chrome's search engine configuration to eliminate having to type `site:about.gitlab.com` every time.  You only have to type 3 characters. Here's how.

**NOTE:** If you are using Firefox, you can use the ["Add custom search engine extension"](https://addons.mozilla.org/en-US/firefox/addon/add-custom-search-engine/) to do this. [Instructions below](#firefox-search).

**First:** Configure a new Search Engine shortcut in Chrome

| Step	 | Image  |
|---------------|----------------|
| 1. Right click on the URL field in Chrome and select "Edit Search Engines  |   ![Edit search engine](/images/handbook/tools-and-tips/searching/1_edit_search_engine.png)  |
| 2. In the Dialog, click `Add`  |   ![Add search engine](/images/handbook/tools-and-tips/searching/2_add_search_engine.png) |
| 3. There are THREE fields in the **Edit search engine** dialog. <br>     a. In the *Search Engine* field Enter `GitLab`<br>     b. In the *Keyword* field, enter `gl`<br>     c. In the *URL* field enter `http://www.google.com/search?q=%s%20site:about.gitlab.com`<br>  d. Click Save. | ![Enter search engine details](/images/handbook/tools-and-tips/searching/3_enter_search_engine_details.png) |

**Then** Go to a new Chrome tab and test it.

| Step	 | Image  |
|---------------|----------------|
| 1. In the Chrome URL/search field type `gl`  | ![Use Keyword to search](/images/handbook/tools-and-tips/searching/4_search_gl.png) |
| 2. AND then press `space`.  Notice how the field changes to indicate the selected search engine. | ![Press space key](/images/handbook/tools-and-tips/searching/5_search_space.png) |
| 3. Now, your **new** GitLab search engine will search using the `site:about.gitlab.com` modifier. | ![Search results from Gitlab](/images/handbook/tools-and-tips/searching/6_search_results.png) |


### What about GitLab documentation?

Simple. Create another search engine.

| Search GitLab Documentation	 | Image  |
|---------------|----------------|
| 1. In the **Edit search engine** dialog. <br>   2. In the *Search Engine* field Enter `GitLab docs` <br>   3. In the *Keyword* field, enter `gd` <br>    4. In the *URL* field enter <br> `http://www.google.com/search?q=%s%20site:docs.gitlab.com` |    ![Settings for docs.gitlab.com](/images/handbook/tools-and-tips/searching/7_gitlab_docs_search.png) |

### What about finding GitLab Issues?

Yep, create another search engine shortcut — this one will search for Issues in gitlab.com

| Search GitLab Issues	 | Image  |
|---------------|----------------|
| 1. In the **Edit search engine** dialog. <br>   2. In the *Search Engine* field Enter `GitLab.com issues` <br>   3. In the *Keyword* field, enter `gg` <br>    4. In the *URL* field enter  <br> `https://gitlab.com/search?search=%s&project_id=&group_id=6543&scope=issues`  (Note this restricts the search to the gitlab.com group) |    ![Settings for docs.gitlab.com](/images/handbook/tools-and-tips/searching/8_gitlab_issues_search.png) |

### What about finding files in Google Docs?

You guessed it. Simply create another search engine shortcut — this one will search for documents in Google Docs

| Search Google Docs	 | Image  |
|---------------|----------------|
| 1. In the **Edit search engine** dialog. <br>   2. In the *Search Engine* field Enter `Google Drive` <br>   3. In the *Keyword* field, enter `dv` <br>    4. In the *URL* field enter <br> `https://drive.google.com/drive/search?q=%s` |    ![Settings for docs.gitlab.com](/images/handbook/tools-and-tips/searching/9_google_drive_search.png) |

### Other advanced search configurations
Below you will find a few more examples of search engine shortcuts you may find useful.  These examples are using the domain `gitlab.com` and the `gitlab-org` project.  These values can be modified to work on your instance URL.

#### Search dotcom-internal issues

| Search Engine | `dotcom-internal issues` |
| Keyword | `ggi` |
| Url | `https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues?scope=all&utf8=%E2%9C%93&state=all&search=%s` |
| Usage | ggi keyword/s |

#### Search open merge requests by author

| Search Engine | `MR Author` |
| Keyword | `mr` |
| Url | `https://gitlab.com/dashboard/merge_requests?scope=all&utf8=%E2%9C%93&state=opened&author_username=%s` |
| Usage | mr username |

#### Search open issues by author

| Search Engine | `Issue Author` |
| Keyword | `author` |
| Url | `https://gitlab.com/dashboard/issues?scope=all&utf8=%E2%9C%93&state=opened&author_username=%s` |
| Usage | author username |

#### Navigate directly to an epic by the known epic number (in gitlab-org project0)

| Search Engine | `GitLab Epic` |
| Keyword | `epic` |
| Url | `https://gitlab.com/groups/gitlab-org/-/epics/%s` |
| Usage | epic 954 |

#### Navigate directly to an issue by the known issue number (in gitlab-org project0)

| Search Engine | `GitLab Issue` |
| Keyword | `Issue` |
| Url | `https://gitlab.com/gitlab-org/gitlab/issues/%s` |
| Usage | issue 31034 |

## Firefox -

### Firefox Bookmarks

In Firefox, it is possible to have the same functionality. The only challenge is in getting to the Firefox settings where you can setup the keywords for searching.


|  Firefox Setup   |     View   |
|------|-----|
|The settings are controlled from the Firefox Bookmark Menu  |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_1_Searching_Overview.png)  |
| 1. Click on the Library Menu icon |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_2_Library_Menu.png)  |
| 2. Click on Show all Bookmarks at the bottom |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_3_Show_all_Bookmarks.png)  |
| 3. Select the Bookmarks Menu item |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_4_Select_Bookmarks_Menu.png)  |
| 4. This is where your search shortcuts live |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_5_Searching.png)  |
| 5. To ADD a new shortcut - Click on the Gear icon and select **New Bookmark** |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_6_New_Bookmark.png)  |
| 7. Give your bookmark/search shortcut a name (any name will do) |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_7_Name_Bookmark.png)  |
| 8. Fill in the details with the URL in the Location field and keyword shortcut in the keyword field |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_8_Bookmark_Details.png)  |
| 9. Use your shortcut, in this case "gg" and a space |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_9_Firefox_Search.png)  |
| Which took me here |  ![Firefox Searching](/images/handbook/tools-and-tips/searching/FF_10_Search_Results.png)  |

### Firefox Import Custom searches 

We can import most of the custom and advanced search we have seen here by doing a direct import, this way we won't have to manually each each one of them.

To do this first we will need the file with the custom search as bookmarks, you can download it from [here](/handbook/tools-and-tips/searching/GitLabSearchShortcuts.html), download that file, and we will use it to load the bookmarks.

With the file download from the [previous tip](https://about.gitlab.com/handbook/tools-and-tips/searching/#firefox-bookmarks), complete step 2 and continue with the following steps.

| Step | Image |
|------|-----|
|Click on the import bookmarks from HTML. | ![Firefox Import Bookmark](/images/handbook/tools-and-tips/searching/FF_Import_bookmarks.png)|

When the file selection dialog open select the file you downloaded earlier and import it to add the following custom search

| Search  | Keyword  |Description   | 
|---|---|---|
|  GitLab Handbook | gl  | Handbook search   |
|  GitLab Documentation | gd |  GitLab documentation [ docs.gitlab.com] | 
| Issues by author  | author  | Search for issues open by given author (username) in all projects  |
| Merge Requests by author   | mr  |  Search for merge requests by given author (username) in all projects |
| Google Drive search  | dv  | Simple google drive search   |


### Firefox Search

Similarly to the Chrome instructions above, you can add a custom search engine into Firefox to allow you to search the handbook (or issues etc) from the address bar.

**First:** Install the ["Add custom search engine extension"](https://addons.mozilla.org/en-US/firefox/addon/add-custom-search-engine/).

**Second:** Configure a new Search Engine shortcut in Firefox

| Step	 | Image  |
|---------------|----------------|
| 1. Click the addon icon in the toolbar or click "Preferences" from the addon manager | ![Add custom search engine extension](/images/handbook/tools-and-tips/searching/1_add_search_engine_firefox.png)  |
| 2. Enter the details for your new search engine <br> a. Enter a useful name <br> b. For the `Search URL` field, enter `http://www.google.com/search?q=%s%20site:about.gitlab.com` <br> c. For the `Icon` field, you can use the GitLab favicon: `https://about.gitlab.com/ico/favicon.ico` | ![Search engine form](/images/handbook/tools-and-tips/searching/2_add_search_engine_firefox.png) |
| 3. Click `Add custom search engine` ||
| 4. Optionally, configure a keyword shortcut by editing the list in `about:preferences#search` ||

**Then:** Go to a new tab, and you will now see an icon for your new search engine at the bottom of the suggestions bar when you enter text in the address bar.

## Using Alfred on macOS

[Alfred](https://www.alfredapp.com/) for macOS

### Using Alfred and Firefox

<!-- blank line -->
<figure class="video_container">
    <iframe src="https://www.youtube.com/embed/tu7YHZAKKN8" frameborder="0" allowfullscreen="true"> </iframe>
  </figure>
  <!-- blank line -->

GitLab team member [Simon M.](https://gitlab.com/simon_mansfield) recorded the video above to walk through the process of searching GitLab like a pro using [Alfred](https://www.alfredapp.com/) (a productivity application for macOS) and the [Firefox web browser](https://www.mozilla.org/en-US/firefox/new/).

### Import these custom searches to Alfred

You can click on each of these URLs and Alfred will ask if you want to import them to your custom searches.
![Add custom search to Alfred](/images/handbook/tools-and-tips/searching/AF_add_to_alfred.png)

| Keyword |
|---------------|
| [gl](alfred://customsearch/gitlab%20handbook/gl/utf8/nospace/https%3A%2F%2Fabout.gitlab.com%2Fhandbook%2F%23stq%3D%7Bquery%7D%26stp%3D1) |
| [gd](alfred://customsearch/gitlab%20docs/gd/utf8/nospace/https%3A%2F%2Fdocs.gitlab.com%2Fsearch%2F%3Fq%3D%7Bquery%7D) |
| [gg](alfred://customsearch/GitLab%20issues%20search/gg/utf8/nospace/https%3A%2F%2Fgitlab.com%2Fsearch%3Fsearch%3D%7Bquery%7D%26project_id%3D%26group_id%3D6543%26scope%3Dissues) |
| [mr](alfred://customsearch/MR%20Author%20GitLab/mr/utf8/nospace/https%3A%2F%2Fgitlab.com%2Fdashboard%2Fmerge_requests%3Fscope%3Dall%26utf8%3D%25E2%259C%2593%26state%3Dopened%26author_username%3D%7Bquery%7D) |
| [author](alfred://customsearch/GitLab%20Issues%20Author/author/utf8/nospace/https%3A%2F%2Fgitlab.com%2Fdashboard%2Fissues%3Fscope%3Dall%26utf8%3D%25E2%259C%2593%26state%3Dopened%26author_username%3D%7Bquery%7D) |
| [issue](alfred://customsearch/GitLab%20issue/issue/utf8/nospace/https%3A%2F%2Fgitlab.com%2Fgitlab-org%2Fgitlab%2Fissues%2F%7Bquery%7D) |

### Add the GitLab icon

You can drag and drop the favicon ![favicon](/ico/favicon-32x32.png) to the Alfred custom search

![](/images/handbook/tools-and-tips/searching/AF_add_icon.png)
