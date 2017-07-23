## Travelify

### Introduction

Travelify is a clean, simple and fully responsive theme for [Pico CMS](http://picocms.org/). It is originally for WordPress by ColorLib ([https://github.com/puikinsh/travelify](https://github.com/puikinsh/travelify)).

### What's supported

 - Global navigation bar
 - Global and page-specific sidebar

### Installation

Download the repo, upload files to corresponding location and change the following setting within your config.php:

    $config['theme'] = 'Travelify';

You also need to add the following new lines:

    $config['site_subtitle'] = 'Another Pico CMS Site';
    $config['site_copyright'] = 'Your Name Here';

Before you continue, make sure that you have copied `content-sample/navbar.md` and `content-sample/slider.md` to your `content` directory.

### Customization

#### Navigation bar

File `content-sample/navbar.md` contains the list of items shown in main navigation bar. You may use Markdown to write a multi-level list there. For example:

	- [Home](%base_url%)
	- [Category 1](#)
		- [Page 1.1](%base_url%?a/a)
			- [Page 1.1.1](%base_url%?a/a/a)
		- [Page 1.2](%base_url%?a/b)
	- [Category 2](#)
		- [Page 2.1](#)
		- [Page 2.2](#)

#### Slider

File `content-sample/slider.md` contains a list of image files as slides.

	*   ![City of Helsinki](%base_url%/assets/slider/uh.jpg)
	*   ![City of Helsinki](%base_url%/assets/slider/uh.jpg)

#### Sidebar

There are two kinds of sidebars, global and page-specific. The global sidebar display on all pages. If one page has its own page-specific sidebar, the latters will be displayed **before** global ones.

Global sidebar is located in `content-sample/sidebars/` folder. You may add prefix to filename in order to maintain sorting.

Example of page-specific sidebars can be found in `content-sample/a/a/sidebars/`. In this example, the sidebar is effective **only** for pages located in `content-sample/a/a` directory, **not** include `content-sample/a/a/a` dictionary.

#### License

The theme is released for free under the terms of the GNU General Public License version 2 and some parts under their respective licenses. In general words, feel free and encouraged to use, modify and redistribute this theme however you like. You may remove any copyright references (unless required by third party components) and crediting is not necessary. The theme is offered free of charge. If someone asked money for it, someone just tricked you.

### Preview

![preview](https://raw.githubusercontent.com/xupefei/Travelify/master/travelify.png)
