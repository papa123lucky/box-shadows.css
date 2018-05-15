# Box-shadows.css <a href="/LICENSE"><img src="http://madeas.ru/img/git/license.svg" alt="license"></a> <a href="/CHANGELOG.md"><img src="http://madeas.ru/img/git/changelog.svg" alt="changelog"></a> <a href="https://github.com/madeas/box-shadows.css/releases"><img src="http://madeas.ru/img/git/release.svg" alt="releases"></a> <a href="https://cdnjs.com/"><img src="http://madeas.ru/img/git/cdnjs.svg" alt="cdn"></a> <a href="https://gitter.im/andrejsharapov/box-shadows.css"><img src="http://madeas.ru/img/git/gitter.svg" alt="chat gitter"></a>
A cross-browser collection of CSS box-shadows. Try, experiment, use whatever you want and how you want!

<code>box-shadows.css</code> a bunch of cool and fun shadows for you to use in your projects. Great for tables, homepages content, containers, navigation and other blocks your website.

## Basic Usage

### 1. Include the stylesheet
1a. Include the stylesheet on your document's <code>&lt;head&gt;</code>
>
    <head>
      <link rel="stylesheet" href="https://madeas.ru/css/box-shadows.css">
    </head>
    
1b. Include the stylesheet minimal css:
>
    <head>
      <link rel="stylesheet" href="https://madeas.ru/css/box-shadows.min.css">
    </head>
    
1c. Download

See [box-shadows.css][link3] and [box-shadows.min.css][link4]
    
1d. Instead of installing you may use the remote version (hosted by CDN):*
>
    <head>
      <link rel="stylesheet" href="../box-shadows.min.css">
    </head>
*in search of cdn platform

### 2. Add the class
Add the class<code>bShadow</code> to the block you want to use.

### 3. Add the class number
Finally you need change <code>bShadow</code> or to add one of the classes. 

Full example:
>
    <div class="bShadow">Example</div> 
or
>   
    <div class="bShadow-1">Example</div>
or
>   
    <div class="bShadow bShadow-1">Example</div>

* Now the collection consists of <b>45 shadows with number</b>, bShadow, bShadow-light and bShadow-inset.

See [example on JSfiddle][link1]

## 4. Hover effect

Add the class <code>h</code> to the element <code>bShadow-1</code> to create an hover effect.

Full example:
>
    <div class="bShadow bShadow-4h">bShadow</div>

See [example on JSfiddle][link2] block one (.bShadow) / try, experiment, use whatever you want and how you want!

## 5. Adding the <code>inset</code> parameter
To add a parameter, just insert the script on the html page and specify in it the classes for which you want to apply it.

Full example for <code>.bShadow-3</code> + <code>.bShadow-4</code>. A point in front of the class is required!
>
    [].forEach.call(document.querySelectorAll('.bShadow-3,.bShadow-4'), function(node) {
	    var bsh = getComputedStyle(node).boxShadow;
	    node.style.boxShadow = "inset "+bsh;
    });
    
 See [example on JSfiddle][link5]

## Animation
Class <code>bShadow</code> uses a smooth default animation in .2s <code>transition: transform 0.2s ease-in-out</code>, and also includes a property that warns the browser about the upcoming shadow transformation and position <code>will-change: transform, box-shadow;</code>.

Use this to make a beautiful animation of your blocks. For example,

>
	<style>
	.transform-translateY-5:hover {
  		-webkit-transform: translateY(-5px) translateZ(0);
  		transform: translateY(-5px) translateZ(0); 
	</style>
	<div class="bShadow transform-translateY-5 bShadow-4h">bShadow</div>
	
See [example on JSfiddle][link5]

## Usage
To use box-shadows.css in your website, simply drop the stylesheet into your document's <code>&lt;head&gt;</code>, and add the class <code>bShadow</code> to an element, along with any of the <code>bShadow-number</code> or singly + <code>hover</code> effect and js <code>inset</code>. Optional. That's all! You've got a CSS block with shadow.

## License
Box-shadows.css.css is licensed under the MIT license. (http://opensource.org/licenses/MIT)

## Contributing
In the process of creating shadow names. I will be grateful for the help.

[link1]: https://jsfiddle.net/madeas/wmreuu2n/
[link2]: https://jsfiddle.net/madeas/wmreuu2n/
[link5]: https://jsfiddle.net/madeas/wmreuu2n/1/
[link3]: https://madeas.ru/css/box-shadows.css
[link4]: https://madeas.ru/css/box-shadows.min.css
