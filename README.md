# Site maintenance notes

These notes describe how to find your way around the implementation of the feeling-responsive Jekyll theme for Victoria's yoga site. Combined with the Google doc shared by Victoria, you should have enough details to maintain this site.

## Configuration
Config details are at jekyll_victoriaheron.com/_config_dev.yml:

### Using two config files for development
Th `_config_dev.yml` file is only needed for development. Instead of changing the url
everytime you work locally on the project, you start the local server with both config-files, overwriting
the first one with the development variables needed.

To start a development server run the following: 
`$ jekyll serve --config _config.yml,_config_dev.yml --incremental`

## Publishing to repo mapping:

```
/ (root) => _layouts/frontpage.html
	image 
	intro text from  
/about => pages/about-me.md

/classes => pages/classes.md

/classes/corporate-classes => _posts/classes/2016-10-02-corporate-classes.md

/classes/private-classes => _posts/classes/2016-10-02-corporate-classes.md

/media - 404
/media/archive - 404
/blog => (builds from /blog/index and /_layouts/blog.htmlblog)
/blog/archive
/contact
	needs wufoo form
```

## Notes:
Need to increase the height value of the masthead element in 
_07_layout.scss and find backstretch to modify it.
