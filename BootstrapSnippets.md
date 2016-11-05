# BootStrap Code
Attached is code for bootstrap.

## Scripts and CSS Links
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
```

## Navbar
<img src="http://brianmikal.com/403midterm/fixednavbar.png" width="650" /><br>
###### Fixed navbar (always showing no matter how you scroll)
```html
<!-- This goes in the beginning of the body tag, if you change the height you must change the body "top" styling -->
<div class="navbar navbar-inverse navbar-fixed-top">
        <div class="container" id="navbartext">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="/">Website Name</a>
            </div>
            <div class="navbar-collapse collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Contact</a></li>
                    <li class="dropdown">
                        <a class="dropdown-toggle" data-toggle="dropdown" href="#">
                            Dropdown
                            <span class="caret"></span>
                        </a>
                        <ul class="dropdown-menu">
                            <li><a href="#">Option 1</a></li>
                            <li><a href="#">Option 2</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
</div>
```


###### Static navbar (scrolls with the page)
```html
<!-- This goes in the beginning of the body tag, if you change the height you must change the body "top" styling -->
<div class="navbar navbar-inverse navbar-static-top">
        <div class="container" id="navbartext">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="/">Website Name</a>
            </div>
            <div class="navbar-collapse collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Contact</a></li>
                    <li class="dropdown">
                        <a class="dropdown-toggle" data-toggle="dropdown" href="#">
                            Dropdown
                            <span class="caret"></span>
                        </a>
                        <ul class="dropdown-menu">
                            <li><a href="#">Option 1</a></li>
                            <li><a href="#">Option 2</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
</div>
```

##### Changing the styling of the navbar
For help picking out a color (or finding out th HEX color) <a href="http://htmlcolorcodes.com/">Click Here</a>

Navbar links:
```css
/* Change background color of navbar (usually make the border-color the same color) */
    .navbar {
    background-color: #09314f;
    border-color: #09314f;
    top:0;
    height: 50px;
        }

/* Change the color of the links on the navbar (only works for navbar that includes the navbar-inverse class) */
    .navbar-inverse .navbar-nav > li > a {
    color: #ffffff;
    font: bolder;
        }
	
/* Change color of the links on the navbar when you hover over them (usually make the border-color the same color) */
    .navbar-inverse .navbar-nav > li:hover {
    background-color: #0a416b;
        }
```


## Buttons

###### Single button
<img src="http://brianmikal.com/403midterm/singlebutton.png" /><br>
```html
<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-primary">Blue</button>

<!-- Color: White -->
<button type="button" class="btn btn-secondary">White</button>

<!-- Color: Green -->
<button type="button" class="btn btn-success">Green</button>

<!-- Color: Light Blue -->
<button type="button" class="btn btn-info">Light Blue</button>

<!-- Color: Yellow -->
<button type="button" class="btn btn-warning">Yellow</button>

<!-- Color: Red -->
<button type="button" class="btn btn-danger">Red</button>

<!-- This is just a button tag that ends up being a link -->
<button type="button" class="btn btn-link">Link</button>

```

###### Button Group

<img src="http://brianmikal.com/403midterm/buttongroup.png" /><br>
```html
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-secondary">Left</button>
  <button type="button" class="btn btn-secondary">Middle</button>
  <button type="button" class="btn btn-secondary">Right</button>
</div>
```


###### Button Dropdown
<img src="http://brianmikal.com/403midterm/buttondropdown.png" /><br>
```html
<div class="dropdown">
    <button class="btn btn-primary dropdown-toggle" type="button" data-toggle="dropdown">Dropdown Example
    <span class="caret"></span></button>
    <ul class="dropdown-menu">
      <li><a href="#">HTML</a></li>
      <li><a href="#">CSS</a></li>
      <li><a href="#">JavaScript</a></li>
    </ul>
  </div>
  ```

## Random Bootstrap

###### Breadcrumbs
<img src="http://brianmikal.com/403midterm/breadcrumbs.png" width="700px" /><br>
```html
<nav class='breadcrumb'><a class='breadcrumb-item' href='#'>Home</a> / <a class='breadcrumb-item' href='#'>Page</a> / <span class='breadcrumb-item active;'>Contact</span></nav>
```
## Panels

###### Collapsing Panels (Clicking on panel headers opens and closes)
<img src="http://brianmikal.com/403midterm/collapsingpanels.png" width="700" /><br>
```html
<div class="container">
  <div class="panel-group" id="accordion">
    <div class="panel panel-default">
      <div class="panel-heading">
        <h4 class="panel-title">
          <a data-toggle="collapse" data-parent="#accordion" href="#collapse1">Collapsible Group 1</a>
        </h4>
      </div>
      <div id="collapse1" class="panel-collapse collapse in">
        <div class="panel-body">Lorem ipsum dolor sit amet, consectetur adipisicing elit,
        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
      </div>
    </div>
    <div class="panel panel-default">
      <div class="panel-heading">
        <h4 class="panel-title">
          <a data-toggle="collapse" data-parent="#accordion" href="#collapse2">Collapsible Group 2</a>
        </h4>
      </div>
      <div id="collapse2" class="panel-collapse collapse">
        <div class="panel-body">Lorem ipsum dolor sit amet, consectetur adipisicing elit,
        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
      </div>
    </div>
    <div class="panel panel-default">
      <div class="panel-heading">
        <h4 class="panel-title">
          <a data-toggle="collapse" data-parent="#accordion" href="#collapse3">Collapsible Group 3</a>
        </h4>
      </div>
      <div id="collapse3" class="panel-collapse collapse">
        <div class="panel-body">Lorem ipsum dolor sit amet, consectetur adipisicing elit,
        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
      </div>
    </div>
  </div>
</div>
```


###### Collapsing Panels (Clicking on button opens and closes div panel)
<img src="http://brianmikal.com/403midterm/simplecollapsible.png" width="700" /><br>
```html
<div class="container">
  <button type="button" class="btn btn-info" data-toggle="collapse" data-target="#demo">Simple collapsible</button>
  <div id="demo" class="collapse">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit,
    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  </div>
</div>
```

###### Simple Panel (rounded border around div)
<img src="http://brianmikal.com/403midterm/simplepanel.png" width="650" /><br>
```html
<div class="panel panel-default">
  <div class="panel-body">A Basic Panel</div>
</div>
```

##Forms
<img src="http://brianmikal.com/403midterm/formpart1.png" width="330" /><br>
<img src="http://brianmikal.com/403midterm/formpart2.png" width="330" /><br>


##### Example Form Setup
```html
<form>
  <div class="form-group">
    <label for="exampleInputEmail1">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
    <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
  </div>
  <div class="form-group">
    <label for="exampleInputPassword1">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
  </div>
  <div class="form-group">
    <label for="exampleSelect1">Example select</label>
    <select class="form-control" id="exampleSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleSelect2">Example multiple select</label>
    <select multiple class="form-control" id="exampleSelect2">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleTextarea">Example textarea</label>
    <textarea class="form-control" id="exampleTextarea" rows="3"></textarea>
  </div>
  <div class="form-group">
    <label for="exampleInputFile">File input</label>
    <input type="file" class="form-control-file" id="exampleInputFile" aria-describedby="fileHelp">
    <small id="fileHelp" class="form-text text-muted">This is some placeholder block-level help text for the above input. It's a bit lighter and easily wraps to a new line.</small>
  </div>
  <fieldset class="form-group">
    <legend>Radio buttons</legend>
    <div class="form-check">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optionsRadios" id="optionsRadios1" value="option1" checked>
        Option one is this and that&mdash;be sure to include why it's great
      </label>
    </div>
    <div class="form-check">
    <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optionsRadios" id="optionsRadios2" value="option2">
        Option two can be something else and selecting it will deselect option one
      </label>
    </div>
    <div class="form-check disabled">
    <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optionsRadios" id="optionsRadios3" value="option3" disabled>
        Option three is disabled
      </label>
    </div>
  </fieldset>
  <div class="form-check">
    <label class="form-check-label">
      <input type="checkbox" class="form-check-input">
      Check me out
    </label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

#####Dropdown list

```html
<form>
  <div class="form-group">
    <label for="exampleSelect1">Example select</label>
    <select class="form-control" id="exampleSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
</form>
```

#####Textarea

```html
<form>
  <div class="form-group">
    <label for="exampleTextarea">Example textarea</label>
    <textarea class="form-control" id="exampleTextarea" rows="3"></textarea>
  </div>
</form>
```

#####Textbox

```html
<form>
    <div class="form-group">
        <label for="exampleTextbox">Example textbox</label>
        <input type="text" class="form-control" placeholder="Placeholder">
    </div>
</form>
```


## Jumbotron
<img src="http://brianmikal.com/403midterm/jumbotron.png" width="550" /><br>

```html
<div class="jumbotron">
            <h1>Big Text</h1>
            <p class="lead">Smaller big text</p>
            <p><a href="#" class="btn btn-primary btn-lg">Learn more &raquo;</a></p>
    </div>  
```
Styling:
```css
/* Current width setting is set to expand across the entire screen, background image can be set to anything */
.jumbotron {
    width: 100%;
    position: relative;
    left: 0;
    background-image:url("http://marriottschool.byu.edu/wp-content/uploads/2015/06/Tanner-1a-1200x506.jpg");
}
```


# ASP.net MVC
The following code is for the .cs or .cshtml files. (AKA Views or Controllers)

## Routing and directing to different views
##### Route Config - Passing paremeters

```cs
// goes in route.config

routes.MapRoute(
                name: "Contact",
                url: "{controller}/{action}/{name}/{email}/{id}",
                defaults: new { controller = "Contact", action = "Index", id = UrlParameter.Optional }
            );
```           
	    
```cs	    
 // URL to pass parameters (first action, then controller, then parameters
@Url.Action("Email","Contact", new { name = "brian", email = "brian@brian.com" })
```


```cs
 // Contact Controllers
using System;
using System.Collections.Generic;
using System.IO;
using System.Linq;
using System.Net;
using System.Net.Mail;
using System.Web;
using System.Web.Mvc;

namespace BlowOut.Controllers
{
    public class ContactController : Controller
    {
        //
        // GET: /Contact/
        public string Email(string name,string email)
        {
            return "<p>Thank you " + name + ". We will send an email to " + email + "</p>";
        }
	}
}
```


##### Route Config - Normal (going to another view)
```cs
// goes in HomeController.cs
public ActionResult About()
        {
            ViewBag.Message = "Your application description page.";
            //load breadcrumb
            ViewBag.breadcrumb = "<nav class='breadcrumb'><a class='breadcrumb-item' href='" + Url.Action("Index", "Home") + "'>Home</a> / <span class='breadcrumb-item active;'>About</span></nav>";
            return View();
        }
```

```cs
//put this in a view to generate the URL for this page
@Url.Action("About")

//put this in a view to generate a complete A tag which includes the URL
@Html.ActionLink("About", "About", "Home")
```

## Referencing documents within the project (the ~ brings you to the root folder)

```cs
~/bundles/modernizr
```


## Loading partial views based on viewbag attributes passed to view
```cs
@if(ViewBag.id == "bsis") {
    Html.RenderPartial("degreeinfo");
}

@if(ViewBag.id == "mism") {
    Html.RenderPartial("degreeinfo");
    }
@if (ViewBag.id != "mism" & ViewBag.id != "bsis") { 
    Html.RenderPartial("selectdegree");
    }

@if (ViewBag.id == "bsis")
{
    <h2>BSIS FAQ's</h2>
    Html.RenderPartial("bsis");
}
```
