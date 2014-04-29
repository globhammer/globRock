globROCK Engine of Rock!!! 
=============

![pixi.js logo](http://www.goodboydigital.com/pixijs/logo_small.png) 

[<img src="http://www.pixijs.com/wp-content/uploads/2013/05/headerPanel_projects-898x342.jpg">](http://www.pixijs.com/projects)
#### Node WebKit Video Game Engine ####

The aim of this project is to provide a method of creating fine art games to be shown in galleries and muesuems for hundreds of years.
globROCK also allows everyone to distrubute webGL games as easily as possible. 
Also, since it built on top of the solid foundation of PIXI.js, its fast.

If you’re interested in the globROCK then feel free to follow the art collective on twitter
([@globHAMMER](https://twitter.com/doormat23)) and we will keep you posted on our progress!  

And of course check back on [our site](<http://www.globHAMMER.com/glob/>) as our process will be discussed there too!

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/GoodBoyDigital/pixi.js/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

### Demos ###

- [ TITLE SCREEN ](<http://www.goodboydigital.com/pixijs/examples/15/indexAll.html>)

Thank you to  :)

### Docs ###

[Documentation can be found here when complete](<http://www.globHAMMER.com/globROCK/docs/>)

### Resources ###

[Tutorial on Set Up](<http://flippinawesome.org/2014/02/10/build-desktop-apps-with-javascript-and-node-webkit/>)

[Pixi.js forum](<http://www.html5gamedevs.com/forum/15-pixijs/>)


### Road Map ###

* New Physics Engine

### Contribute ###

Want to be part of globHAMMER? Great! All are welcome! We will get to the globenHIEM quicker together :P
Whether you find a bug, have a great feature request or you fancy owning a task from the road map above feel free to get in touch.

Make sure to read the [Contributing Guide](https://github.com/globHAMMER/globROCK/glob/master/CONTRIBUTING.md) before submitting changes.

### How to Play ###

Install Node.js
http://nodejs.org/download/

Using the Command Line Interface install the Grunt CLI globally by typing
```
$> npm install –g grunt-cli
```



Then, in the folder where you have downloaded the source, install the build dependencies using npm:

```
$> npm install
```

Then build:

```
$> grunt
```

This will create a minified version at bin/pixi.js and a non-minified version at bin/pixi.dev.js.

It also copies the non-minified version to the examples.

### Current features ###

- WebGL renderer (with automatic smart batching allowing for REALLY fast performance)
- Canvas renderer (Fastest in town!)
- Full scene graph
- Super easy to use API (similar to the flash display list API)
- Support for texture atlases
- Asset loader / sprite sheet loader
- Auto-detect which renderer should be used
- Full Mouse and Multi-touch Interaction
- Text
- BitmapFont text
- Multiline Text
- Render Texture
- Spine support
- Primitive Drawing
- Masking
- Filters

### Usage ###

```javascript

	// You can use either PIXI.WebGLRenderer or PIXI.CanvasRenderer
	var renderer = new PIXI.WebGLRenderer(800, 600);

	document.body.appendChild(renderer.view);

	var stage = new PIXI.Stage;

	var bunnyTexture = PIXI.Texture.fromImage("bunny.png");
	var bunny = new PIXI.Sprite(bunnyTexture);

	bunny.position.x = 400;
	bunny.position.y = 300;

	bunny.scale.x = 2;
	bunny.scale.y = 2;

	stage.addChild(bunny);

	requestAnimationFrame(animate);

	function animate() {
		bunny.rotation += 0.01;

		renderer.render(stage);

		requestAnimationFrame(animate);
	}
```

This content is released under the (http://opensource.org/licenses/MIT) MIT License.

[![Analytics](https://ga-beacon.appspot.com/UA-39213431-2/pixi.js/index)](https://github.com/igrigorik/ga-beacon)!!!!
