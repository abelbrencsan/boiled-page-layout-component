# Boiled Page layout component

Layout SCSS component for Boiled Page frontend framework. It is intended to structure page into a aside and a main column. The former one can be on the left or the right side, sticky parts can be defined inside it, or it can be even skipped.

## Install

Place `_layout.scss` file to `/assets/css/components` directory, and add its path to components block in `assets/css/app.scss` file.

## Usage

### Classes

Class name | Description | Example
---------- | ----------- | -------
`layout` | Applies layout. | `<div class="accordion"></div>`
`layout-aside` | Applies aside column inside layout. | `<aside class="accordion-aside"></aside>`
`is-important` | Modifies position of aside over main on medium or smaller breakpoints. | `<aside class="accordion-aside is-important"></aside>`
`layout-aside-sticky` | Applies a sticky part inside aside. | `<div class="layout-aside-sticky"></div>`
`layout-main` | Applies main column inside layout. | `<main class="accordion-main"></main>`

### Examples

#### Example 1

The following example shows a layout with sticky aside on the left side, and a main on the right one. The former one is positioned under the latter one from medium breakpoint.

```html
<div class="layout">

  <!-- Layout aside -->
  <aside class="layout-aside">
    <div class="layout-aside-sticky">
      <div class="box">
        <p>Dolores reiciendis molestias optio quos quasi minus quas.</p>
      </div>
    </div>
  </aside>

  <!-- Layout main -->
  <main class="layout-main">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam volutpat porta turpis a ultricies. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla blandit mauris ut nisi laoreet, et lacinia tellus mattis. Proin sodales sit amet enim commodo imperdiet. Donec id mollis augue, a consequat lectus. Nam eget blandit tortor. Phasellus hendrerit est nec lacus placerat interdum. In non aliquam risus, sed bibendum ex. Nullam placerat auctor urna suscipit lacinia. In dapibus nisl augue, varius pellentesque dolor bibendum non. Quisque sed erat purus. Fusce risus nunc, efficitur vel orci et, tincidunt suscipit justo. Integer quis suscipit sapien, vitae pretium urna. Praesent in mollis dolor, sit amet hendrerit risus. Maecenas non risus vel urna lacinia semper.</p>
  </main>
  
</div>
```

#### Example 2

The following example shows a layout with a main on the left side and an aside on the right one. The latter one is positioned over the former one from medium breakpoint.

```html
<div class="layout">

  <!-- Layout main -->
  <main class="layout-main">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam volutpat porta turpis a ultricies. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla blandit mauris ut nisi laoreet, et lacinia tellus mattis. Proin sodales sit amet enim commodo imperdiet. Donec id mollis augue, a consequat lectus. Nam eget blandit tortor. Phasellus hendrerit est nec lacus placerat interdum. In non aliquam risus, sed bibendum ex. Nullam placerat auctor urna suscipit lacinia. In dapibus nisl augue, varius pellentesque dolor bibendum non. Quisque sed erat purus. Fusce risus nunc, efficitur vel orci et, tincidunt suscipit justo. Integer quis suscipit sapien, vitae pretium urna. Praesent in mollis dolor, sit amet hendrerit risus. Maecenas non risus vel urna lacinia semper.</p>
  </main>

  <!-- Layout aside -->
  <aside class="layout-aside is-important">
    <div class="box">
      <p>Dolores reiciendis molestias optio quos quasi minus quas.</p>
    </div>
  </aside>
  
</div>
```
