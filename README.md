# ![LOGO](logo.png) Figshare **flow**ground Connector

## Description

A generated **flow**ground connector for the Figshare API (version 2.0.0).

Generated from: https://api.apis.guru/v2/specs/figshare.com/2.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:40:43+03:00

## API Description

Figshare apiv2. Using Swagger 2.0

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Private Account information

> Account information for token/personal token

*Tags:* `other`

### Private Articles

> Get Own Articles

*Tags:* `articles`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit

### Create new Article

> Create a new Article by sending article information

*Tags:* `articles`

### Private Articles search

> Returns a list of private articles filtered by the search parameters

*Tags:* `articles`

### Delete article

> Delete an article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Article details

> View a private article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Update article

> Updating an article by passing body parameters

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### List article authors

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Add article authors

> Associate new authors with the article. This will add new authors to the list of already associated authors

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Replace article authors

> Associate new authors with the article. This will remove all already associated authors and add these new ones

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Delete article author

> De-associate author from article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `author_id` - _required_ - Article Author unique identifier

### List article categories

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Add article categories

> Associate new categories with the article. This will add new categories to the list of already associated categories

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Replace article categories

> Associate new categories with the article. This will remove all already associated categories and add these new ones

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Delete article category

> De-associate category from article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `category_id` - _required_ - Category unique identifier

### Delete article confidentiality

> Delete confidentiality settings

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Article confidentiality details

> View confidentiality settings

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Update article confidentiality

> Update confidentiality settings

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Delete Article Embargo

> Will lift the embargo for the specified article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Article Embargo Details

> View a private article embargo details

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Update Article Embargo

> Note: setting an article under whole embargo does not imply that the article will be published when the embargo will expire. You must explicitly call the publish endpoint to enable this functionality.

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### List article files

> List private files

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Initiate Upload

> Initiate new file upload within the article. Either use link to provide only an existing file that will not be uploaded on figshare or use the other 3 parameters(md5, name, size)

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### File Delete

> Complete file upload

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `file_id` - _required_ - File unique identifier

### Single File

> View details of file for specified article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `file_id` - _required_ - File unique identifier

### Complete Upload

> Complete file upload

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `file_id` - _required_ - File unique identifier

### List private links

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Create private link

> Create new private link for this article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Disable private link

> Disable/delete private link for this article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `link_id` - _required_ - Private link token

### Update private link

> Update existing private link for this article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier
* `link_id` - _required_ - Private link token

### Private Article Publish

> - If the whole article is under embargo, it will not be published immediatly, but when the embargo expires or is lifted.<br/>
> - When an article is published, a new public version will be generated. Any further updates to the article will affect the private article data. In order to make these changes publicly visible, an explicit publish operation is needed.

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Private Article Reserve DOI

> Reserve DOI for article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article unique identifier

### Search Authors

> Search for authors

*Tags:* `authors`

### Author details

> View author details

*Tags:* `authors`

#### Input Parameters
* `author_id` - _required_ - Author unique identifier

### Private Account Categories

> List institution categories (including parent Categories)

*Tags:* `institutions`

### Private Collections List

> List private collections

*Tags:* `collections`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.

### Create collection

> Create a new Collection by sending collection information

*Tags:* `collections`

### Private Collections Search

> Returns a list of private Collections

*Tags:* `collections`

### Delete collection

> Delete n collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Collection details

> View a collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Update collection

> Update collection details

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### List collection articles

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Add collection articles

> Associate new articles with the collection. This will add new articles to the list of already associated articles

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Replace collection articles

> Associate new articles with the collection. This will remove all already associated articles and add these new ones

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Delete collection article

> De-associate article from collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier
* `article_id` - _required_ - Collection article unique identifier

### List collection authors

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Add collection authors

> Associate new authors with the collection. This will add new authors to the list of already associated authors

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Replace collection authors

> Associate new authors with the collection. This will remove all already associated authors and add these new ones

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Delete collection author

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier
* `author_id` - _required_ - Collection Author unique identifier

### List collection categories

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Add collection categories

> Associate new categories with the collection. This will add new categories to the list of already associated categories

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Replace collection categories

> Associate new categories with the collection. This will remove all already associated categories and add these new ones

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Delete collection category

> De-associate category from collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier
* `category_id` - _required_ - Collection category unique identifier

### List collection private links

> List article private links

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Create collection private link

> Create new private link

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier

### Disable private link

> Disable/delete private link for this collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier
* `link_id` - _required_ - Private link token

### Update collection private link

> Update existing private link for this collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection unique identifier
* `link_id` - _required_ - Private link token

### Private Collection Publish

> When a collection is published, a new public version will be generated. Any further updates to the collection will affect the private collection data. In order to make these changes publicly visible, an explicit publish operation is needed.

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Private Collection Reserve DOI

> Reserve DOI for collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Private Account Institutions

> Account institution details

*Tags:* `institutions`

### Private Account Institution Accounts

> Returns the accounts for which the account has administrative privileges (assigned and inherited).

*Tags:* `institutions`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `is_active` - _optional_ - Filter by active status
* `institution_user_id` - _optional_ - Filter by institution_user_id
* `email` - _optional_ - Filter by email

### Create new Institution Account

> Create a new Account by sending account information

*Tags:* `institutions`

### Private Account Institution Accounts Search

> Returns the accounts for which the account has administrative privileges (assigned and inherited).

*Tags:* `institutions`

### Update Institution Account

*Tags:* `institutions`

#### Input Parameters
* `account_id` - _required_ - Account identifier the user is associated to

### Private Institution Articles

> Get Articles from own institution. User must be administrator of the institution

*Tags:* `institutions`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.
* `published_since` - _optional_ - Filter by article publishing date. Will only return articles published after the date. date(ISO 8601) YYYY-MM-DD
* `modified_since` - _optional_ - Filter by article modified date. Will only return articles published after the date. date(ISO 8601) YYYY-MM-DD
* `status` - _optional_ - only return collections with this status
* `resource_doi` - _optional_ - only return collections with this resource_doi
* `item_type` - _optional_ - Only return collections with the respective type. Mapping for item_type is: 1 - Figure, 2 - Media, 3 - Dataset, 4 - Fileset, 5 - Poster, 6 - Paper, 7 - Presentation, 8 - Thesis, 9 - Code, 11 - Metadata, 12 - Preprint

### Private Account Institution Groups

> Returns the groups for which the account has administrative privileges (assigned and inherited).

*Tags:* `institutions`

### Private Account Institution Roles

> Returns the roles available for groups and the institution group.

*Tags:* `institutions`

### List Institution Account Group Roles

*Tags:* `institutions`

#### Input Parameters
* `account_id` - _required_ - Account identifier the user is associated to

### Add Institution Account Group Roles

*Tags:* `institutions`

#### Input Parameters
* `account_id` - _required_ - Account identifier the user is associated to

### Delete Institution Account Group Role

*Tags:* `institutions`

#### Input Parameters
* `account_id` - _required_ - Account identifier for which to remove the role
* `group_id` - _required_ - Group identifier for which to remove the role
* `role_id` - _required_ - Role identifier

### Private Account Institution User

> Retrieve institution user information using the account_id

*Tags:* `institutions`

#### Input Parameters
* `account_id` - _required_ - Account identifier the user is associated to

### Private Account Licenses

> This is a private endpoint that requires OAuth. It will return a list with figshare public licenses AND licenses defined for account's institution.

*Tags:* `other`

### Private Projects

> List private projects

*Tags:* `projects`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.
* `storage` - _optional_ - only return collections from this institution
    Possible values: group, individual.
* `roles` - _optional_ - Any combination of owner, collaborator, viewer separated by comma. Examples: "owner" or "owner,collaborator".

### Create project

> Create a new project

*Tags:* `projects`

### Private Projects search

> Search inside the private projects

*Tags:* `projects`

### Delete project

> A project can be deleted only if: - it is not public - it does not have public articles.<br/>
> <br/>
> When an individual project is deleted, all the articles are moved to my data of each owner.<br/>
> <br/>
> When a group project is deleted, all the articles and files are deleted as well. Only project owner, group admin and above can delete a project.

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### View project details

> View a private project

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### Update project

> Updating an project by passing body parameters

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### List project articles

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Proejct unique identifier

### Create project article

> Create a new Article and associate it with this project

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Proejct unique identifier

### Delete project article

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `article_id` - _required_ - Project Article unique identifier

### Project article details

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `article_id` - _required_ - Project Article unique identifier

### Project article list files

> List article files

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `article_id` - _required_ - Project Article unique identifier

### Project article file details

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `article_id` - _required_ - Project Article unique identifier
* `file_id` - _required_ - File unique identifier

### List project collaborators

> List Project collaborators and invited users

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### Invite project collaborators

> Invite users to collaborate on project or view the project

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### Remove project collaborator

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `user_id` - _required_ - User unique identifier

### Private Project Leave

> Please note: project's owner cannot leave the project.

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### List project notes

*Tags:* `projects`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit

### Create project note

> Create a new project note

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### Delete project note

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `note_id` - _required_ - Note unique identifier

### Project note details

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `note_id` - _required_ - Note unique identifier

### Update project note

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier
* `note_id` - _required_ - Note unique identifier

### Private Project Publish

> Publish a project. Possible after all items inside it are public

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project unique identifier

### Public Articles

> Returns a list of public articles

*Tags:* `articles`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.
* `institution` - _optional_ - only return collections from this institution
* `published_since` - _optional_ - Filter by article publishing date. Will only return articles published after the date. date(ISO 8601) YYYY-MM-DD
* `modified_since` - _optional_ - Filter by article modified date. Will only return articles published after the date. date(ISO 8601) YYYY-MM-DD
* `group` - _optional_ - only return collections from this group
* `resource_doi` - _optional_ - only return collections with this resource_doi
* `item_type` - _optional_ - Only return collections with the respective type. Mapping for item_type is: 1 - Figure, 2 - Media, 3 - Dataset, 4 - Fileset, 5 - Poster, 6 - Paper, 7 - Presentation, 8 - Thesis, 9 - Code, 11 - Metadata, 12 - Preprint
* `doi` - _optional_ - only return collections with this doi

### Public Articles Search

> Returns a list of public articles, filtered by the search parameters

*Tags:* `articles`

### View article details

> View an article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier

### List article files

> Files list for article

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier

### Article file details

> File by id

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier
* `file_id` - _required_ - File Unique identifier

### List article versions

> List public article versions

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier

### Article details for version

> Article with specified version

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier
* `v_number` - _required_ - Article Version Number

### Public Article Confidentiality for article version

> Confidentiality for article version

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier
* `v_number` - _required_ - Version Number

### Public Article Embargo for article version

> Embargo for article version

*Tags:* `articles`

#### Input Parameters
* `article_id` - _required_ - Article Unique identifier
* `v_number` - _required_ - Version Number

### Public Categories

> Returns a list of public categories

*Tags:* `other`

### Public Collections

> Returns a list of public collections

*Tags:* `collections`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.
* `institution` - _optional_ - only return collections from this institution
* `published_since` - _optional_ - Filter by collection publishing date. Will only return collections published after the date. date(ISO 8601) YYYY-MM-DD
* `modified_since` - _optional_ - Filter by collection modified date. Will only return collections published after the date. date(ISO 8601) YYYY-MM-DD
* `group` - _optional_ - only return collections from this group
* `resource_doi` - _optional_ - only return collections with this resource_doi
* `doi` - _optional_ - only return collections with this doi

### Public Collections Search

> Returns a list of public collections

*Tags:* `collections`

### Collection details

> View a collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Public Collection Articles

> Returns a list of public collection articles

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit

### Collection Versions list

> Returns a list of public collection Versions

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier

### Collection Version details

> View details for a certain version of a collection

*Tags:* `collections`

#### Input Parameters
* `collection_id` - _required_ - Collection Unique identifier
* `version_id` - _required_ - Version Number

### Public File Download

> Starts the download of a file

*Tags:* `other`

#### Input Parameters
* `file_id` - _required_

### Private Institution HRfeed Upload

> More info in the <a href="#hr_feed">HR Feed section</a>

*Tags:* `institutions`

### Public Licenses

> Returns a list of articles belonging to the institution

*Tags:* `institutions`

#### Input Parameters
* `institution_string_id` - _required_
* `resource_id` - _required_
* `filename` - _required_

### Public Licenses

> Returns a list of public licenses

*Tags:* `other`

### Public Projects

> Returns a list of public projects

*Tags:* `projects`

#### Input Parameters
* `page` - _optional_ - Page number. Used for pagination with page_size
* `page_size` - _optional_ - The number of results included on a page. Used for pagination with page
* `limit` - _optional_ - Number of results included on a page. Used for pagination with query
* `offset` - _optional_ - Where to start the listing(the offset of the first result). Used for pagination with limit
* `order` - _optional_ - The field by which to order. Default varies by endpoint/resource.
    Possible values: published_date, modified_date, views, shares, downloads, cites.
* `order_direction` - _optional_
    Possible values: asc, desc.
* `institution` - _optional_ - only return collections from this institution
* `published_since` - _optional_ - Filter by article publishing date. Will only return articles published after the date. date(ISO 8601) YYYY-MM-DD
* `group` - _optional_ - only return collections from this group

### Public Projects Search

> Returns a list of public articles

*Tags:* `projects`

### Public Project

> View a project

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project Unique identifier

### Public Project Articles

> List articles in project

*Tags:* `projects`

#### Input Parameters
* `project_id` - _required_ - Project Unique identifier

## License

**flow**ground :- Telekom iPaaS / figshare-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
