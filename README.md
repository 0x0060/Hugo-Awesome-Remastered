# Blog Setup Guide

This guide will walk you through the process of cloning and setting up the blog repository, installing a theme, and running the blog locally using Hugo. It also includes instructions for customizing your theme for easy setup.

## Prerequisites

Before starting, ensure you have the following installed on your local machine:

- [Git](https://git-scm.com/downloads)
- [Hugo](https://gohugo.io/getting-started/installing/)

## Setup Instructions

### 1. Clone the Blog Repository

Start by cloning the main blog repository to your local machine:

&&&
git clone https://github.com/0x0060/Blog-Template
&&&

### 2. Navigate to the `themes` Directory

Move into the `themes` directory inside the cloned `Blog` project:

&&&
cd Blog/themes
&&&

### 3. Clone the Hugo-Awesome-Remastered Theme

Clone the Hugo-Awesome-Remastered theme into the `themes` directory and rename it as `Hugo-Awesome-Remastered`:

&&&
git clone https://github.com/0x0060/Hugo-Awesome-Remastered.git Hugo-Awesome-Remastered
&&&

### 4. Navigate Back to the Root Directory

Once the theme is successfully cloned, move back to the root directory of the blog project:

&&&
cd ..
&&&

### 5. Configure Theme Support

Hugo-Awesome-Remastered comes with easy customization options. To enable the theme and configure it, open the `config.toml` file in the root directory and ensure it contains the following:

&&&
theme = "Hugo-Awesome-Remastered"
&&&

This will tell Hugo to use the `Hugo-Awesome-Remastered` theme for your blog.

### 6. Run the Blog Locally

To start the Hugo development server and preview your blog locally, run the following command:

&&&
hugo serve
&&&

### Accessing Your Local Blog

Once the server is running, you should see an output like this:

&&&
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop the server.
&&&

Now, open your web browser and navigate to `http://localhost:1313/` to view your local blog.

---

## Customizing Your Theme

The Hugo-Awesome-Remastered theme allows for easy customization, so you can adjust the design and settings based on your preferences.

1. **Update the `config.toml` File**  
   The `config.toml` file contains important settings for your blog, including title, description, social links, and more. Open it and update the following fields to match your blog's details:

&&&
title = "My Awesome Blog"
description = "This is a description of my awesome Hugo blog"
author = "Your Name"
&&&

2. **Add Custom Content**  
   You can add your own pages or posts by creating new Markdown files in the `content` directory. For example, to add a new post, navigate to:

&&&
content/posts/my-first-post.md
&&&

Add your content using Markdown syntax.

3. **Theme Customization**  
   The theme supports various customizations such as changing colors, fonts, and layout options. Check the theme documentation for a detailed list of configuration options. Customize the appearance by modifying the relevant files inside the `themes/Hugo-Awesome-Remastered` directory.

For more details on how to customize Hugo themes, check the official documentation [here](https://gohugo.io/getting-started/configuration/).
