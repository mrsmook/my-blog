
#### Understanding the configuration variables

The configuration variables referenced above are used as follows:

| Variable | Description of Use |
|----------|--------------------|
| title | The title of the blog. This is used for the page title primarily. |
| author | The author of the blog. This is used for the header name and page title. |
| description | The description of the author. This is used for the header under the author. |
| primaryColor | The primary color of the blog. |
| showHeaderImage | Flag to show the header image or not. |
| showShareButtons  | Flag to show social media share buttons on each blog post or not. |
| postsPerPage | The number of posts per page on the blog homepage. This is used for pagination. |
| social | Social media profiles of the blog author. Currently only personal website, Github, Twitter, and LinkedIn are supported.|

#### Changing the main header image

To change the default header image, simply override the ```main.jpg``` file in the ```/src``` folder.

#### Changing the favicon

To change the default favicon, simply override the ```favicon.ico``` file in the ```/src``` folder.

## Creating New Posts

All blog posts can be found in ```/src/pages``` and are statically built once the ```gatsby build``` command is run. To create a new post, simply create a new folder in ```/src/pages``` with the name of the url you'd like to have. For example, if you wish to have the url appear as ```myblog.com/hello-world``` you would create the folder as ```hello-world```. Once the folder is created, simply create an ```index.md``` file within it.

The top of the pages must all contain the same markdown which tells Gatsby the needed information about the specific post. The basic template is:

```markdown
---
title: New Beginnings
date: "2018-07-01"
featuredImage: './featured.jpg'
---

This top portion is the beginning of the post and will show up as the excerpt on the homepage.

<!-- end -->
```

In the above code snippet all that is required is the **title** and the **date**. The featured image is optional and can be added by simply adding an image to the page folder you just created and referencing like the above example. The excerpt portion is optional as well and if you do not use the ```<!-- end -->``` marker, the first bit of the post will be used as the excerpt automatically.

This template ships with 3 blog post examples which contain everything from code snippet usage, inserting images, using featured images and excerpts, and more.

## Deploying

Once you are ready to deploy the blog and make it live, you have a couple of options available to you.
