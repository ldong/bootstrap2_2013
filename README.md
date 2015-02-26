# Bootstrap 2 for 2013

Note and source code for: Bootstrap for Web Design 2013

Date: Wed Feb 25 04:52:58 PST 2015

See my new notes for **bootstrap3** [here](https://github.com/ldong/bootstrap3_2015)
# Notes

# Basic Div
* container container-fluid
* row row-fluid
* fluid is **12** for sure
* non-fluid is fixed

## Base class

### Texts
* text-error
* text-warning
* text-info
* text-success

* muted
* text-left
* text-right
* text-center

### Block quotes
block quotes use for citation

```html
<blockquote class='pull-right'>
    <p> Texts </p>
    <small>John Doe from <cite title='Source Title'>Great Source</cite> </small>
</blockquote>
```

### List
```html
<ul class='unstyled'>
    <li> </li>
    <li> </li>
    <li> </li>
</ul>

<ol>
    <li> </li>
    <li> </li>
    <li> </li>
</ol>

<ol class='inline'>
    <li> </li>
    <li> </li>
    <li> </li>
</ol>

// usually for Questions and Answers
<dl class=='dl-horizontal'>
    <dt>Term</dt>
    <dd>Description</dd>
</dl>
```
### Table
```html
<table class="table table-bordered table-condensed">
    <caption>This is a default table</caption>
    <thead>
        <tr>
            <th>#</th>
            <th>First Name</th>
            <th>Last Name</th>
        </tr>
    </thead>
    <tbody>
        <tr class="success">
            <td>1</td>
            <td>Adi</td>
            <td>Purdila</td>
        </tr>
        <tr class="error">
            <td>2</td>
            <td>John</td>
            <td>Smith</td>
        </tr>
        <tr class="warning">
            <td>1</td>
            <td>Adi</td>
            <td>Purdila</td>
        </tr>
        <tr class="info">
            <td>1</td>
            <td>Adi</td>
            <td>Purdila</td>
        </tr>
    </tbody>
</table>
```

#### Optional class
```html
class='table-striped'
class='table-bordered'
class='table-hovered'
class='table-condensed'

class="success"
class="error"
class="warning"
class="info"
```

### Button

```html
<a href='' class='btn'> </a>
<button class='btn'> </button>

<input type='text' class='btn' value='Input Text' />
<input type='submit' class='btn' value='Submit Input' />

// Colors
class="btn-primary"
class="btn-info"
class="btn-success"
class="btn-warning"
class="btn-danger"

class='btn-inverse'
class='btn-link'

// Sizes
class='btn-large'
class='btn-small'
class='btn-mini'

class='btn-block'
```

anchor tag <- disabled

button <- disabled or class='disabled'
<button class='btn' disabled> </button>
<button class='btn disabled' disabled> </button>

## Images
```html
<img src='http://link.com' alt='demo' class='img-rouned' />
<img src='http://link.com' alt='demo' class='img-circle' />
<img src='http://link.com' alt='demo' class='img-polarized' />
```

## Icons
```html
<i class='icon-music'> </i>

<a href='' class='btn btn-primary'> Music
    <i class='icon-music icon-white'></i>
</a>

<a href='' class='btn btn-primary'>
    <i class='icon-music icon-white'></i> Music
</a>
```

## Form Controls
### Text Input
### Text Area

### Checkbox
```html
<label class='checkbox'> <input type='checkbox'/>Simple Checkbox</label>
<label class='radio'> <input type='radio'/>Simple radio</label>

```
### Raido button
```html
<label class='radio inline'> <input type='radio'/>Simple radio</label>
<label class='radio inline'> <input type='radio'/>Simple radio</label>
<label class='radio inline'> <input type='radio'/>Simple radio</label>
<label class='radio inline'> <input type='radio'/>Simple radio</label>
```

1. help-inline
2. help-block

```html
<form class='form-inline'>
    <label for='simple-input'>Simple Text Input </label>
    <input type='text' id='simple-input' name='simple-input'
    paceholder='Type something' />
    <span class='help-inline'>Some descriptions here</span>
</form>
```

### Control Sizing

class:

1. span
2. input-block-level

```html
<input class="input-mini" type="text"/>
<input class="input-small" type="text"  />
<input class="input-medium" type="text" />
<input class="input-large" type="text"  />
<input class="input-xlarge" type="text" />
<input class="input-xxlarge" type="text"/>

// without clear overflow
<input type='text' class='span6' />
<input type='text' class='span6' />

// remove overflow
<div class='controls control-row'>
    <input type='text' class='span2' />
    <input type='text' class='span3' />
    <input type='text' class='span5' disabled/>
</div>
```

Valid email

```html
<form>
    <input type='email' id='simple-input' name='simple-input'
    placeholder='Enter your email' class='input-block-level' required />
</form>
```

input with warning

```html
<div class='control-group warning'>
    <label for='input-warning' class='control-label'>
    input with warning</label>
    <div class='controls'>
        <input type='text' id='input-warning'/>
        <span class='help-block'>Some descriptions here</span>
    </div>
</div>
```

## Extending Form Controls
```html
<form>
    <div class='input-prepend'>
        <span class='add-on'>Enter email here</span>
        <input type='text' placeholder='Enter Here' class='input-block-level' required />
    </div>

    <div class='input-append'>
        <input type='text' placeholder='Enter Here' class='input-block-level' required />
        <span class='add-on'>Enter email</span>
    </div>

    <div class='input-append input-prepend'>
        <span class='add-on'>Enter email here</span>
        <input type='text' placeholder='Enter Here' class='input-block-level' required />
        <span class='add-on'>Enter email</span>
    </div>
</form>
```

### Form Layouts
1. Search form
    ```html
    <form>
        <input type='text' />
        <button type='submit' class='btn'>Search</button>
    </form>

    <form class=form-search"">
        <input type='text' class='search-quer'/>
        <input type='submit' class='btn'> Search</button>
    </form>
    ```

2.  Inline form
    ```html
    <form class='form-inline'>
        <input type='email' placeholder='Email'/>
        <input type='password' placeholder='password'/>

        <label class='checkbox'>
            <input type='checkbox' /> Remember me
        </label>
        <button type='submit' class='btn'>Search</button>
    </form>
    ```


3.  horizontal form
    ```html
    <form class='form-horizontal'>
        <div class='control-group'>
            <label class="control-label">Email</label>
            <div class="controls">
                <input type='email' placeholder='Email'/>
            </div>
        </div>
        <div class='control-group'>
            <label class="control-label">Password</label>
            <div class="controls">
                <input type='password' placeholder='Password'/>
            </div>
        </div>

        <div class='control-group'>
            <div class="controls">
                <label class='checkbox'>
                <input type='checkbox' /> Remember me </label>
                <button type='submit' class='btn'>Search</button>
            </div>
        </div>
    </form>
    ```

## DropDown
```html
<div class='container'>
    <div class="dropdown">
        <a class='dropdownToggle' data-toggle='dropdown'
        href="#">Dropdown <b class="caret"></b></a>
        <ul class="dropdown-menu pull-right">
        	<li><a href="" tabindex="-1">Action 1</a></li>
        	<li class='dropdown-submenu'>
                <a href="" tabindex="-1">Action 2</a>
                <ul class="dropdown-menu">
                	<li><a href="" tableindex="-1">sub1</a></li>
                	<li><a href="" tableindex="-1">sub2</a></li>
                	<li><a href="" tableindex="-1">sub3</a></li>
                </ul>
            </li>
            <li class="divider"></li>
        	<li class='disabled'><a href="" tabindex="-1">Action 3</a></li>
        </ul>
    </div>
</div>
```

Pull right: `<ul class="dropdown-menu pull-right">`


## button groups and button dropdown

div>button.btn{Button}*3
```html
<div class='btn-group btn-group-vertical'>
	<button class="btn">Button</button>
	<button class="btn">Button</button>
	<button class="btn">Button</button>
</div>

<div class='btn-toolbar'>
    <div class='btn-group'>
        <button class="btn">Button</button>
        <button class="btn">Button</button>
        <button class="btn">Button</button>
    </div>

    <div class='btn-group'>
        <button class="btn">Button</button>
        <button class="btn">Button</button>
        <button class="btn">Button</button>
    </div>
</div>


<div>
    <button type='button' id='loading-button' class="btn" data-loading-text='Loading'>
        Loading Button
    </button>
</div>
```

With additional JavaScript
```js
(function(){
    $('#loading-button').click(function(){
        var btn = $(this);
        btn.button('loading');
        setTimeout(function(){
            btn.button('reset');
        }, 1000);
    })
})();
```

```html
<button class="btn" data-toggle="button">Google Chrome</button>

<div class='btn-group' data-toggle='buttons-checkbox'>
    <button class="btn">Button</button>
    <button class="btn">Button</button>
    <button class="btn">Button</button>
</div>

<div class='btn-group' data-toggle='buttons-radio'>
    <button class="btn">Button</button>
    <button class="btn">Button</button>
    <button class="btn">Button</button>
</div>
```

### Button dropdown menu
```html
<div class="btn-group">
    <button class="btn btn-primary" data-toggle='dropdown'>DropDown Menu <b class="caret"></b> </button>
    <ul class="dropdown-menu">
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    </ul>
</div>

<div class="btn-group">
    <button class="btn btn-primary btn-large dropdown-toggle" data-toggle='dropdown'>DropDown Menu <b class="caret"></b> </button>
    <ul class="dropdown-menu">
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    </ul>
</div>
```

`class='dropdown-toggle'`, make it dropdown like

`data-toggle='dropdown'`, make it actually clickable


```html
<div class="btn-group">
    <button class="btn">DropDown Menu</button>
	<button class="btn dropdown-toggle" data-toggle='dropdown'><span class="caret"></span></button>
    <ul class="dropdown-menu">
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    	<li><a href="">Link</a></li>
    </ul>
</div>
```

```html
<div class="btn-group dropup">
    <button class="btn">DropDown Menu</button>
	<button class="btn dropdown-toggle" data-toggle='dropdown'><span class="caret"></span></button>
    <ul class="dropdown-menu">
    	<li><a href="">Link</a></li>
    	<li><a hre f="">Link</a></li>
    	<li><a href="">Link</a></li>
    </ul>
</div>

```

## Tabs and Pills
Tabs

```html
<ul class='nav nav-tabs'>
	<li class='active'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
</ul>
```

Pills

```html
<ul class='nav nav-pills'>
	<li class='active'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li class='disabled'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
</ul>
```

Stacked
```html
<ul class='nav nav-tabs nav-stacked'>
	<li class='active'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
</ul>
```

Dropdown

```html
<ul class='nav nav-tabs'>
	<li class='active'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li class='dropdown'>
        <a class='dropdown-toggle' data-toggle='tab' href="">Dropdown
        <b class="caret"></b></a>
        <ul class="dropdown-menu">
        	<li><a href="tabindex-1">Sublink1</a></li>
        	<li><a href="tabindex-1">Sublink1</a></li>
        	<li><a href="tabindex-1">Sublink1</a></li>
        </ul>
    </li>
</ul>
```


Tabs with Tab content
```html
<div class="container">
    <ul class='nav nav-tabs'>
        <li class='active'><a href="#tab1" data-toggle='tab'>Link1</a></li>
        <li><a href="#tab2" data-toggle='tab'>Link2</a></li>
        <li><a href="#tab3" data-toggle='tab'>Link3</a></li>
        <li><a href="#tab4" data-toggle='tab'>Link3</a></li>
        <li class='dropdown'>
            <a class='dropdown-toggle' data-toggle='dropdown' href="">Dropdown
                <b class="caret"></b></a>
            <ul class="dropdown-menu">
                <li><a href="" tabindex-1="">Sublink1</a></li>
                <li><a href="" tabindex-1="">Sublink2</a></li>
                <li><a href="" tabindex-1="">Sublink3</a></li>
            </ul>
        </li>
    </ul>

    <div class="tab-content">
        <div class="tab-pane active" id='tab1'>
            <p>Tab Content 1</p>
        </div>
        <div class="tab-pane" id='tab2'>
            <p>Tab Content 2</p>
        </div>
        <div class="tab-pane" id='tab3'>
            <p>Tab Content 3</p>
        </div>
        <div class="tab-pane" id='tab4'>
            <p>Tab Content 4</p>
        </div>
    </div>
</div>
```

Tabbable

* tab-right
* tab-left
* tab-below, in this, the *tab content* must be on top of *navs*
```html
<div class='tabbable'>
    /// contents
</div>
```

Nav list 
```html
<ul class='nav nav-list'>
	<li class='nav-header'>Header1</li>
	<li class='active'><a href="">Link</a></li>
	<li><a href="">Link</a></li>
	<li class='nav-header'>Header2</li>
	<li><a href="">Link</a></li>
	<li class='disabled'><a href="">Link</a></li>
    <li class="divider"></li>
	<li>
        <a href="">Link</a>
        <ul class="nav nav-list">
        	<li><a href="">Sublink1</a></li>
        	<li><a href="">Sublink2</a></li>
        </ul>
    </li>
</ul>
```
## Nav Bar
Nav bar

```html
<div class=container>
    <div class="navbar">
    	<div class="navbar-inner">
            <a class="brand" href="">Project Name</a>
            <ul class="nav">
            	<li><a href="">Link 1</a></li>
            	<li><a href="">Link 2</a></li>
                <li class="divider-vertical"></li>
            	<li><a href="">Link 3</a></li>
            	<li><a href="">Link 4</a></li>
            </ul>
            <form class="navbar-form" action="">
            	<input type="text" placeholder='search here'/>
            	<button type='submit' class='btn'>Search</button>
            </form>

            <form class="navbar-search pull-right" action="">
            	<input type="text" placeholder='search here' class='search-query'/>
            </form>

            <p class="navbar-text">This is a text</p>
        </div>
    </div>
</div>
```

Display variations

* navbar navbar-fixed-top
* navbar navbar-fixed-bottom

```html
<div class="navbar nav-fixed-top">
	<div class="navbar-inner">
		<div class="container">
            <a class="brand" href="">Project Name</a>
            <ul class="nav">
            	<li><a href="">Link 1</a></li>
            	<li><a href="">Link 2</a></li>
                <li class="divider-vertical"></li>
            	<li><a href="">Link 3</a></li>
            	<li><a href="">Link 4</a></li>
            </ul>
            <form class="navbar-form" action="">
            	<input type="text" placeholder='search here'/>
            	<button type='submit' class='btn'>Search</button>
            </form>

            <form class="navbar-search pull-right" action="">
            	<input type="text" placeholder='search here' class='search-query'/>
            </form>

            <p class="navbar-text">This is a text</p>
        </div>
	</div>
</div>
```

Color of Navbar

```html
<div class="navbar nav-fixed-top navbar-inverse">
```

Responsive bar

1. Must include responsive.css

```html
<a class="btn btn-navbar" data-toggle='collapse' data-target='.nav-collapse'>
Show content</a>
<div class="collapse nav-collapse">
    <p class='navbar-text'> This will be hidden less than 940px</p>
</div>
```

## breadcrumb
Used to show hierarchy-based information

![](http://www.tutorialspoint.com/bootstrap/images/breadcrumb_demo.jpg)

```html
<div class="container">
    <ul class="breadcrumb">
    <li><a href="">Link 1</a>
        <span class="divider">/</span>
    </li>
    <li class='active'>Link 2</li>
    <li><a href="">Link 3</a></li>
    </ul>
</div>
```

## Pagination Control
Pagination

```html
<div class="pagination pagination-large">
	<ul>
		<li class='active'><a href="">List 1</a></li>
		<li class='disabled'><a href="">List 2</a></li>
		<li><a href="">List 3</a></li>
		<li><a href="">List 4</a></li>
		<li><a href="">List 5</a></li>
	</ul>
</div>
```

Pager

```html
<ul class="pager">
	<li><a href="">Prev</a></li>
	<li><a href="">Next</a></li>
</ul>

<ul class="pager">
	<li class="previous disabled"><a href="">Prev</a></li>
	<li class="next"><a href="">Next</a></li>
</ul>
```

## Labels and Badges

Labels

```html
<div class="container">
    <span class="label">Default</span>
    <span class="label label-success">Success</span>
    <span class="label label-warning">Warning</span>
    <span class="label label-important">Important</span>
    <span class="label label-info">Info</span>
    <span class="label label-inverse">Info</span>
</div>
```

Badges

```html
<div class="container">
	<span class="badge badge-success">1</span>
	<span class="badge badge-warning">2</span>
	<span class="badge badge-important">3</span>
	<span class="badge badge-info">4</span>
	<span class="badge badge-inverse">5</span>
</div>

```

Heading

```html
<div class='container'>
    <div class="hero-unit">
        <h1>Big Title Here</h1>
        <p>This is a tagline</p>
    </div>
    <div class='page-header'>
        <h1>This is a page header <small>Said hello</small></h1>
    </div>
</div>
```

## Alert and Progress Bars

Alert
```html
<div class='container'>
    <div class="alert">
        <a class="close" data-dismiss="alert" href="">&times;</a>
        Some text
    </div>
    <div class="alert alert-block">
        <a class="close" data-dismiss="alert" href="">&times;</a>
        Some text
    </div>
    <div class="alert alert-block alert-error">Some text</div>
    <div class="alert alert-block alert-success">Some text</div>
    <div class="alert alert-block alert-warning">Some text</div>
</div>
```

Progress Bar
```html
<div class='progress'>
    <div class="bar" style="width:60%"></div>
</div>

<div class='progress progress-striped'>
    <div class="bar" style="width:60%"></div>
</div>

<div class='progress progress-striped active'>
    <div class="bar" style="width:60%"></div>
</div>
```
## Well and Thumbnails
Well

```html
<div class="container">
	<div class="well well-large">Bigger Well</div>
	<div class="well">Some Text</div>
	<div class="well well-small">Small Well</div>
</div>
```
Thumbnails

Thumbnails in list

```html
<ul class="thumbnails">
	<li><a class="thumbnail" href=""><img src="http://lorempixel.com/200/200" alt=""></a></li>
	<li><a class="thumbnail" href=""><img src="http://lorempixel.com/200/200" alt=""></a></li>
	<li><a class="thumbnail" href=""><img src="http://lorempixel.com/200/200" alt=""></a></li>
	<li><a class="thumbnail" href=""><img src="http://lorempixel.com/200/200" alt=""></a></li>
</ul>
```
Thumbnails in Div

```html
<ul class="thumbnails">
	<li class="span3">
		<div class="thumbnail">
			<h3>title</h3>
			<p>some text</p>
		</div>
	</li>
	<li class="span3">
		<div class="thumbnail">
			<h3>title</h3>
			<p>some text</p>
		</div>
	</li>
	<li class="span3">
		<div class="thumbnail">
			<h3>title</h3>
			<p>some text</p>
		</div>
	</li>
	<li class="span3">
		<div class="thumbnail">
			<h3>title</h3>
			<p>some text</p>
		</div>
	</li>
</ul>
```
