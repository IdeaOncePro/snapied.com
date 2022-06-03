# Snapied #1 design tool
## _Easy to Use Online Graphic Designing Platform_

[![N|Snapied design tool](https://www.snapied.com/assets/images/snapied-logo.svg)](https://www.snapied.com)


[Snapied](https://www.snapied.com) is a simple yet powerful online graphic design tool that helps both professional and non-designers create amazing designs easily and quickly.

## Snapied Giant toolbox, beautiful designs, almost no learning curve

>  Let Snapied do the work for you and you focus on what's important in your life. Snapied is an online design tool that helps anyone design beautiful design with minimal effort.


- Remove Background
Removing the image background is just one click away
- Quotes
With over 250,000 quotes from the world's greatest minds and iconic figures, Snapied's database has something for everyone.
- Photo Shapes & Frames
Simply select any photo from the photo gallery and add a cool frame or mask to it from the editor toolbar. All frames are free!
- HD Download
Snapied offers the following formats: JPG, PNG, SVG, WebP, PDF (single and multiple pages), Transparent images and the quality scale ranges from 1x to 5x.
- Brand workspaces
Each workspace can be designed for a specific purpose and can contain its own assets, designs, and team members, and you can switch between workspaces anytime.
- Branding or Design Presets
Save your brand's fonts, colors, logo, and logo position for a unified look across all designs. Snapied doesn't restrict you on the number of brands you create.
- Discover Templates
Templates are pre-built design elements that contain text, photos, frames, tables, shapes, and other objects. You can use templates to create polished documents quickly.
- Color Palettes
Color is an important decision, which is why we've developed Palettes. Make perfect color combinations for your unique style with Color Palettes.
- Perfect Free Images & Backgrounds
You can search for beautiful, high-quality images from a variety of sources and use them.
- Icons
These are the most useful and unique sets of icons. The goal is to inspire creativity with these fun, unique icons.
- Illustrations & Elements
The Snapied design tool is a collection of illustrations, elements, and icons that can be used in any creative context.
- Color picker
This tool helps you pick the color from any object present in your design.
- Fonts & Custom Fonts
Snapied lets you select a font from a list of common fonts, You can upload your own fonts
- Backgrounds
Add backgrounds to your design with a single click
- Texts & Templates
Add text to your photos and create messages that will last forever. Make your messages stand out.
- Design Layers
Use the layers panel to change the visibility of objects, lock transformations on selected layers, or show or hide objects.
- Multiple Pages
Create multiple pages within one design, and Snapied makes it easier to share the content across each platform.
- Image Filters
Enhance your photos with Snapied filters.
- Resize your design
Snapied allows you to resize your design from any size to a specific size in a jiffy.
- Split a picture into Pieces
Grids of different sizes can be chosen as per the requirement along with the output format of your choice (e.g jpeg, or png).
- Drawing tools
Snapied design tool provides multiple Pen tools to suit your use cases and creative style 
- Favorite items
You can mark a template, image, illustration, quote, etc you favorite to use later.
- Copy & paste on Snapied canvas
Copy or drag&drop the image from anywhere into Snapied canvas.
- White label Graphic Design 🎁
You need a graphic design editor that is white label, so it can be embedded into your website or platform. Snapied is for you!






- ✨Magic ✨

## Features

- Import a HTML file and watch it magically convert to Markdown
- Drag and drop images (requires your Dropbox account be linked)
- Import and save files from GitHub, Dropbox, Google Drive and One Drive
- Drag and drop markdown and HTML files into Dillinger
- Export documents as Markdown, HTML and PDF

Markdown is a lightweight markup language based on the formatting conventions
that people naturally use in email.
As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually- written in Markdown! To get a feel
for Markdown's syntax, type some text into the left window and
watch the results in the right.

## Tech

Dillinger uses a number of open source projects to work properly:

- [AngularJS] - HTML enhanced for web apps!
- [Ace Editor] - awesome web-based text editor
- [markdown-it] - Markdown parser done right. Fast and easy to extend.
- [Twitter Bootstrap] - great UI boilerplate for modern web apps
- [node.js] - evented I/O for the backend
- [Express] - fast node.js network app framework [@tjholowaychuk]
- [Gulp] - the streaming build system
- [Breakdance](https://breakdance.github.io/breakdance/) - HTML
to Markdown converter
- [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

## Installation

Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.

Install the dependencies and devDependencies and start the server.

```sh
cd dillinger
npm i
node app
```

For production environments...

```sh
npm install --production
NODE_ENV=production node app
```

## Plugins

Dillinger is currently extended with the following plugins.
Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:

```sh
node app
```

Second Tab:

```sh
gulp watch
```

(optional) Third:

```sh
karma test
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```

## License

MIT

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
