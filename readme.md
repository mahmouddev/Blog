# Blog module

[![Latest Version](https://img.shields.io/github/release/asgardcms/blog.svg?style=flat-square)](https://github.com/asgardcms/blog/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Quality Score](https://img.shields.io/scrutinizer/g/asgardcms/blog.svg?style=flat-square)](https://scrutinizer-ci.com/g/asgardcms/blog)
[![SensioLabs Insight](https://img.shields.io/sensiolabs/i/c54f38d9-20fb-41e8-b2be-bdeb7144ad4b.svg)](https://insight.sensiolabs.com/projects/c54f38d9-20fb-41e8-b2be-bdeb7144ad4b)
[![CodeClimate](https://img.shields.io/codeclimate/github/AsgardCms/Blog.svg)](https://codeclimate.com/github/AsgardCms/Blog)

[![Total Downloads](https://img.shields.io/packagist/dd/asgardcms/blog-module.svg?style=flat-square)](https://packagist.org/packages/asgardcms/blog-module)
[![Total Downloads](https://img.shields.io/packagist/dm/asgardcms/blog-module.svg?style=flat-square)](https://packagist.org/packages/asgardcms/blog-module)
[![Total Downloads](https://img.shields.io/packagist/dt/asgardcms/blog-module.svg?style=flat-square)](https://packagist.org/packages/asgardcms/blog-module)
[![Slack](http://slack.asgardcms.com/badge.svg)](http://slack.asgardcms.com/)


## Installation

Execute the following command in your terminal

    composer require asgardcms/blog-module


Followed by a composer update

**Note: After installation you'll have to give you the required permissions to get to the blog module pages in the backend.**


## Usage

- You have to create a `blog.index` and `blog.show` page in your front end theme.
- You can link to the blog index page using : `route(locale() . '.blog')`
- In the blog index you'll have access to a `$posts` variable on which you can loop
- To create a link to a specific post: `route(locale() . '.blog.slug', [$post->slug])`
- On the blog index and blog show pages you'll have access to a `$latestPosts` variable containing the latest posts, this amount can be configured in the admin.
- On a post detail page, you can have access to the next and previous post by calling:
    - `$post->present()->previous`
    - `$post->present()->next`


## Resources

- [View the changelog](CHANGELOG.md)
- [Contribute to AsgardCMS](CONTRIBUTING.md)
- [License](LICENSE.md)


## Info

All AsgardCMS modules respect [Semantic Versioning](http://semver.org/).
