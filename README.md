# Responsive Nav Example

Since some frameworks lack this, a responsive nav menu in vanilla CSS.

## Installation
- Clone the repo: `git clone https://github.com/GreenSoap/responsive-nav-example`
- It will clone to the current directory, cd to responsive-nav-example
- Run: `npm install`
- Install the Live Server extension in VSCode's marketplace and click "Go Live" in the right hand corner.

## The trick

```html
<input type="checkbox" id="mobile-menu-checkbox">
<label for="mobile-menu-checkbox" class="mobile-menu-toggler">Menu</label>
<ul class="nav-menu">...</ul>
```

```css
#mobile-menu-checkbox:not(:checked) ~ .nav-menu {
  display: none;
}

#mobile-menu-checkbox:checked ~ .nav-menu {
  display: block;
}
```
