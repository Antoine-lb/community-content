![Tutorials](/assets/banner-tutorials.png)

# Tutorials

Follow along with our community tutorials to get you up and running with Strapi: [https://strapi.io/tutorials](https://strapi.io/tutorials)

## How to add a tutorial

There are different cases for adding a tutorial:

1. You want to list an **existing tutorial** on the web
   - Edit the `tutorials.yml` file by adding the tutorial.
2. You want to add your own tutorial
   - [How to write a tutorial](#how-to-write-a-tutorial)

### How to request a tutorial

- Create an issue with the template [Request a tutorial](https://github.com/strapi/community-content/issues/new?assignees=Mcastres&labels=To+do&template=request-a-tutorial.md&title=%5BREQUEST%5D)
- Assign all the necessary labels including the `To do` label

### How to consult tutorials ideas

- Go on the Github repository and consult either the issue or the project

## How to write a tutorial

If you intend to create a tutorial, please check our [guidelines](https://github.com/strapi/community-content/blob/master/tutorials/GUIDELINES.md) first.

There are different cases:

1. The tutorial hasn't been proposed yet
   - Create an issue with the template `Create a tutorial`
   - Create a new branch: `git checkout -b create/<name-of-tutorial>`
   - Create the tutorial and make a pull request by adding a new folder inside `tutorials/code` containing the code of your tutorial as well as editing the `tutorials.yml` file by listing your creation.
   - We will update the issue from **In progress** to **Done**
2. The tutorial is looking for an author (you are doing a requested tutorial)
   - Create a new branch: `git checkout -b create/<name-of-tutorial>`
   - Create the tutorial and make a pull request by adding a new folder inside `tutorials/code` containing the code of your tutorial as well as editing the `tutorials.yml` file by listing your creation.
   - We will update the issue from **Looking for author** to **Done**

**Please follow this format and indentation:**

```yaml
- title: Building a Static Blog using Gatsby and Strapi
 link: https://blog.strapi.io/building-a-static-website-using-gatsby-and-strapi/
 formats:
   - article
 language: en
 date: 2018-01-18
 authors:
   - David Kartuzinski
 github_authors:
   - davidkartuzinski
 source: https://blog.strapi.io/
 image_url: https://blog.strapi.io/content/images/2018/11/gatsby-strapi.png
 use_case: "Blog"
 stack: 
   - Gatsby
 version: beta
```

- `title` - Title of tutorial (`string`; **required**)
- `link` - Working URL where tutorial can be found (`string`; **required**)
- `formats` - Media format of tutorial (`array` of `strings` with values `video`, `audio` or `article`; **required**)
- `language` - Spoken/written language of the tutorial (`string` with a two-letter [ISO 639-1 language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes); optional)
- `date` - Date tutorial was published (`string` in `YYYY-MM-DD` format; optional)
- `authors` - Name of author(s) or speaker(s) (`array` of `strings`; **required**)
- `github_authors` - Github username of author(s) or speaker(s) (`array` of `strings`; optional)
- `source` - Source of the tutorial (`string`; optional)
- `image_url` - Url image of the tutorial (`string`; optional)
- `use_case` - Use case for this tutorial (`strings`; **required**)
- `stack` - Main stack used in the tutorial (`array` of `strings`; **required**)
- `version` - Version of Strapi used in the tutorial (`string`; require)

## Why write for us?

Here are few things that writing for strapi can do for you:

- Learn while sharing your knowledge. You know how to create an application with Strapi and Nuxt? Pass this knowledge to others!
- Get your name on this repository README.md
- Get a complete Strapi course

**By making a tutorial for us you participate in the growth of an open source project.**
