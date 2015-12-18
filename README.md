# Webcomponent

## 什么是webcomponent
长期以来开发者常常以插件或模块的方式来共享代码片段，开发时可以重用这些功能片段。这种方式持续了很长时间，在必要的地方通过引入javascipt、css和html片段。同时你又希望这些引入的文件不会与你的网站或app产生冲突。webcomponent就能很好的解决这个问题，通过对代码进行封装，每个component维护自己的hmtl、style和javascript，不会对外部的环境产生冲突

## important concepts
To understand the webcomponent well, you need know the following core concepts

### html template
定义了&lt;template&gt;标签,方便基于DOM的模板操作

### Custom Element
是开发者可以自己定义并扩展html标签

### shadow DOM
Shadow DOM gives us the best features of iframes, style and markup encapsulation, without nearly as much bloat.

#### Shadow Host
In shadow DOM parlance, the element that you call createShadowRoot on is known as the Shadow Host. It's the only piece visible to the user, and it's where you would ask the user to supply your element with content

#### shadow Root
The document fragment returned by createShadowRoot is known as the Shadow Root. The shadow root, and its descendants, are hidden from the user, but they're what the browser will actually render when it sees our tag

#### Shadow Boundary
Any HTML and CSS inside of the shadow root is protected from the parent document by an invisible barrier called the Shadow Boundary. The shadow boundary prevents CSS in the parent document from bleeding into the shadow DOM, and it also prevents external JavaScript from traversing into the shadow root.

### Html Import
打包组件，并通过&lt;link&gt;标签导入组件


<p data-height="268" data-theme-id="0" data-slug-hash="eJZEBq" data-default-tab="result" data-user="ShirlyFE" class='codepen'><a href='http://codepen.io/ShirlyFE/pen/eJZEBq/'>See a simple component demo </a> by shirly (<a href='http://codepen.io/ShirlyFE'>@ShirlyFE</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

<iframe height="268" scrolling="no" src='//codepen.io/ShirlyFE/embed/eJZEBq/?height=268&theme-id=0&default-tab=result' frameborder="no" allowtransparency="true" allowfullscreen="true" style="width: 100%;"></iframe>See the Pen <a href='http://codepen.io/ShirlyFE/pen/eJZEBq/'>eJZEBq</a> by shirly (<a href='http://codepen.io/ShirlyFE'>@ShirlyFE</a>) on <a href="http://codepen.io">CodePen</a>.

## resources

[A Guide to Web Components](https://css-tricks.com/modular-future-web-components/)

[Shadow DOM](http://www.html5rocks.com/en/tutorials/webcomponents/shadowdom/)