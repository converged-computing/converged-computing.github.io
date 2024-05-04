---
layout: docs
title:  "Examples Page"
tagline: "Examples for how to show site content."
sections:
  - Class Reference
  - Usage
  - Compiled Example
---

# Alerts


<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.alert</td><td class="result">the base alert class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.alert-{{ item.name }}</td><td class="result">{{ item.name }} theme color</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
```html
<div class="alert alert-primary">
  This is a primary alert—check it out!
</div>
<div class="alert alert-secondary">
  This is a secondary alert—check it out!
</div>
<div class="alert alert-success">
  This is a success alert—check it out!
</div>
<div class="alert alert-danger">
  This is a danger alert—check it out!
</div>
<div class="alert alert-warning">
  This is a warning alert—check it out!
</div>
<div class="alert alert-info">
  This is a info alert—check it out!
</div>
<div class="alert alert-light">
  This is a light alert—check it out!
</div>
<div class="alert alert-dark">
  This is a dark alert—check it out!
</div>
```

<div class="alert alert-primary">
  This is a primary alert—check it out!
</div>
<div class="alert alert-secondary">
  This is a secondary alert—check it out!
</div>
<div class="alert alert-success">
  This is a success alert—check it out!
</div>
<div class="alert alert-danger">
  This is a danger alert—check it out!
</div>
<div class="alert alert-warning">
  This is a warning alert—check it out!
</div>
<div class="alert alert-info">
  This is a info alert—check it out!
</div>
<div class="alert alert-light">
  This is a light alert—check it out!
</div>
<div class="alert alert-dark">
  This is a dark alert—check it out!
</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="alert alert-primary"><strong>Well done!</strong> You successfully read this important alert message.</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="alert alert-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate !important; width: 100%; border: 0;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 4px; color: #012e70; margin: 0; padding: 12px 20px; border: 1px solid transparent;" align="left" bgcolor="#d7e7ff">
        <div>
          <strong>Well done!</strong> You successfully read this important alert message.
        </div>
      </td>
    </tr>
  </tbody>
</table>
```


# Badges

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.badge</td><td class="result">the base badge class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.badge-{{ item.name }}</td><td class="result">{{ item.name }} theme color</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Use the [Background Color](/docs/background-color), [Text Color](/docs/text-color), and [Border Radius](/docs/border-radius) classes to style badges.

```html
<span class="badge bg-primary">Primary</span>
<span class="badge bg-secondary">Secondary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning text-dark">Warning</span>
<span class="badge bg-info text-dark">Info</span>
<span class="badge bg-light text-dark rounded-full">Light</span>
<span class="badge bg-dark rounded-full">Dark</span>
```

<span class="badge bg-primary">Primary</span>
<span class="badge bg-secondary">Secondary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning text-dark">Warning</span>
<span class="badge bg-info text-dark">Info</span>
<span class="badge bg-light text-dark rounded-pill">Light</span>
<span class="badge bg-dark rounded-pill">Dark</span>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="badge badge-primary">Badge</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="badge badge-primary" align="left" role="presentation" border="0" cellpadding="0" cellspacing="0">
  <tbody>
    <tr>
      <td style="line-height: 1; font-size: 75%; display: inline-block; font-weight: 700; white-space: nowrap; border-radius: 4px; margin: 0; padding: 4px 6.4px;" align="center" valign="baseline">
        <span>Badge</span>
      </td>
    </tr>
  </tbody>
</table>
```

# Align-X

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.ax-left</td><td class="result">align horizontally left</td></tr>
      <tr><td class="class">.ax-right</td><td class="result">align horizontally right</td></tr>
      <tr><td class="class">.ax-center</td><td class="result">align horizontally center</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Align uses the `align="left|center|right` property on `table` to align anything horizontally. When it is used with a `table` or `td` it will put that property directly on them, however if it is used on any other tag it will wrap that element with a `table` and align it accordingly.
```html
<div class="ax-left">Align left on all viewport sizes</div><br>
<div class="ax-right">Align right on all viewport sizes</div><br>
<div class="ax-center">Align center on all viewport sizes</div>
<a class="btn btn-primary ax-right" href="http://bootstrapemail.com">Right Aligned Button</a>
```

<div class="float-start">Align left on all viewport sizes</div><br>
<div class="float-end">Align right on all viewport sizes</div><br>
<div class="d-table mx-auto position-relative">Align center on all viewport sizes</div>
<a class="btn btn-primary float-end" href="http://bootstrapemail.com">Right Aligned Button</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="ax-left">Hello</div>
<div class="ax-center">WOWWWWW</div>
<div class="ax-right">Goodbye</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="ax-left" role="presentation" align="left">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">Hello</div>
      </td>
    </tr>
  </tbody>
</table>

<table class="ax-center" role="presentation" align="center" style="margin: 0 auto;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">WOWWWWW</div>
      </td>
    </tr>
  </tbody>
</table>

<table class="ax-right" role="presentation" align="right">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">Goodbye</div>
      </td>
    </tr>
  </tbody>
</table>
```

# Align-Y

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.ay-top</td><td class="css">vertical-align: top;</td></tr>
      <tr><td class="class">.ay-middle</td><td class="css">vertical-align: middle;</td></tr>
      <tr><td class="class">.ay-bottom</td><td class="css">vertical-align: bottom;</td></tr>
      <tr><td class="class">.ay-baseline</td><td class="css">vertical-align: baseline;</td></tr>
      <tr><td class="class">.ay-text-top</td><td class="css">vertical-align: text-top;</td></tr>
      <tr><td class="class">.ay-text-bottom</td><td class="css">vertical-align: text-bottom;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Vertical align allows you to vertically align the contents of a table cell. It can only be use in conjunction with a table cell. However most parts of Bootstrap Email are converted into tables so it can feel pretty automatic. You can also apply them directly to the parent `table` to adjust all of the `td` vertical alignments. If you are looking to vertically align child elements of a Stack, check out the [alignment section](/docs/stack#alignment) of the Stack docs.
```html
<table class="h-24">
  <tbody>
    <tr>
      <td class="ay-baseline">baseline</td>
      <td class="ay-top">top</td>
      <td class="ay-middle">middle</td>
      <td class="ay-bottom">bottom</td>
      <td class="ay-text-top">text-top</td>
      <td class="ay-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>
```

<table style="height: 96px;">
  <tbody>
    <tr>
      <td class="align-baseline">baseline</td>
      <td class="align-top">top</td>
      <td class="align-middle">middle</td>
      <td class="align-bottom">bottom</td>
      <td class="align-text-top">text-top</td>
      <td class="align-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<table class="h-24">
  <tbody>
    <tr>
      <td class="ay-baseline">baseline</td>
      <td class="ay-top">top</td>
      <td class="ay-middle">middle</td>
      <td class="ay-bottom">bottom</td>
      <td class="ay-text-top">text-top</td>
      <td class="ay-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="h-24" border="0" cellpadding="0" cellspacing="0" style="height: 96px;" height="96">
  <tbody>
    <tr>
      <td class="ay-baseline" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="baseline" height="96">baseline</td>
      <td class="ay-top" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="top" height="96">top</td>
      <td class="ay-middle" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="middle" height="96">middle</td>
      <td class="ay-bottom" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="bottom" height="96">bottom</td>
      <td class="ay-text-top" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="text-top" height="96">text-top</td>
      <td class="ay-text-bottom" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="text-bottom" height="96">text-bottom</td>
    </tr>
  </tbody>
</table>
```

# Background Color

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.bg-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td><td style="background-color: {{ item.color  }};"></td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.bg-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td><td style="background-color: {{ item.color  }};"></td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Since emails render mostly consistently with tables, many of the components are built into tables. These color classes apply to the current element as well as the child `<td>` so you can use it on a component it will still work if the component is compiled into a table. It also uses the `bgcolor` property for support for old email clients. If a background color utility class is used on a `<div>` it will automatically be converted to a table with 100% width since divs don't have good background color support in many email clients.
```html
<div class="bg-primary text-white">.bg-primary</div>
<div class="bg-secondary text-white">.bg-secondary</div>
<div class="bg-success text-white">.bg-success</div>
<div class="bg-red-500 text-white">.bg-red-500</div>
<div class="bg-yellow-500 text-white">.bg-yellow-500</div>
```

<div class="bg-primary text-white">.bg-primary</div>
<div class="bg-secondary text-white">.bg-secondary</div>
<div class="bg-success text-white">.bg-success</div>
<div class="bg-danger text-white">.bg-red-500</div>
<div class="bg-warning text-white">.bg-yellow-500</div>

{% include header.html name="Customize" hr="true" %}
See the [Customize](/docs/customize) docs to learn more about customizing the color palette.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="bg-blue-100">Blue 100</div>
<div class="bg-blue-200">Blue 200</div>
<div class="bg-blue-300">Blue 300</div>
<div class="bg-blue-400">Blue 400</div>
<div class="bg-blue-500">Blue 500</div>
<div class="bg-blue-600">Blue 600</div>
<div class="bg-blue-700">Blue 700</div>
<div class="bg-blue-800">Blue 800</div>
<div class="bg-blue-900">Blue 900</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="bg-blue-100 w-full" role="presentation" style="width: 100%;" bgcolor="#cfe2ff" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#cfe2ff" width="100%">
        Blue 100
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-200 w-full" role="presentation" style="width: 100%;" bgcolor="#9ec5fe" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#9ec5fe" width="100%">
        Blue 200
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-300 w-full" role="presentation" style="width: 100%;" bgcolor="#6ea8fe" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#6ea8fe" width="100%">
        Blue 300
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-400 w-full" role="presentation" style="width: 100%;" bgcolor="#3d8bfd" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#3d8bfd" width="100%">
        Blue 400
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-500 w-full" role="presentation" style="width: 100%;" bgcolor="#0d6efd" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#0d6efd" width="100%">
        Blue 500
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-600 w-full" role="presentation" style="width: 100%;" bgcolor="#0a58ca" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#0a58ca" width="100%">
        Blue 600
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-700 w-full" role="presentation" style="width: 100%;" bgcolor="#084298" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#084298" width="100%">
        Blue 700
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-800 w-full" role="presentation" style="width: 100%;" bgcolor="#052c65" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#052c65" width="100%">
        Blue 800
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-900 w-full" role="presentation" style="width: 100%;" bgcolor="#031633" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#031633" width="100%">
        Blue 900
      </td>
    </tr>
  </tbody>
</table>
```

# Block

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">&lt;block&gt;, .to-table</td><td class="result">turn the current element into a table and move the classes onto the table.</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Since many email clients have poor support for block elements such as `div`s, `table`s are usually used in their place. Much of Bootstrap Email automatically builds things into tables automatically and applies the correct styles. However there are certain time when that is not the case and you want to easy make something into a table without having to write out the full table structure.

This is where `block` or `.to-table` come in. `block` is an HTML element and `to-table` is a class but both have the same result of turning the current element into a table.
```html
<!-- these two examples are equivalent -->
<div class="to-table w-full border-3 border-red-300">Hello</div>
<block class="w-full border-3 border-red-300">Hello</block>
```

Tip: Use the `w-full` class to make a table `width: 100%` to make it work like a div or block element.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="to-table w-full border-3 border-red-300">Hello</div>
<block class="w-full border-3 border-red-300">Hello</block>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="to-table w-full border-3 border-red-300" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; border: 3px solid #ea868f;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" width="100%">
        Hello
      </td>
    </tr>
  </tbody>
</table>
<table class="w-full border-3 border-red-300 to-table" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; border: 3px solid #ea868f;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" width="100%">
        Hello
      </td>
    </tr>
  </tbody>
</table>
```

# Border Color

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      {% for color in site.data.theme_colors %}
        <tr><td class="class">.border-{{ color.name }}</td><td class="css">border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
      {% for color in site.data.palette_colors %}
        <tr><td class="class">.border-{{ color.name }}</td><td class="css">border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>


# Border

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for border in site.data.border_widths %}
        <tr><td class="class">.border{{ border.name }}</td><td class="css">border: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-top{{ border.name }}</td><td class="css">border-top: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-right{{ border.name }}</td><td class="css">border-right: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-bottom{{ border.name }}</td><td class="css">border-bottom: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-left{{ border.name }}</td><td class="css">border-left: {{ border.width }}px solid #dee2e6;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>

# Border Radius

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for border in site.data.border_radiuses %}
        <tr><td class="class">.rounded{{ border.name }}</td><td class="css">border-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-top{{ border.name }}</td><td class="css">border-top-left-radius: {{ border.radius }}px;<br>border-top-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-right{{ border.name }}</td><td class="css">border-top-right-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-bottom{{ border.name }}</td><td class="css">border-bottom-left-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-left{{ border.name }}</td><td class="css">border-top-left-radius: {{ border.radius }}px;<br>border-bottom-left-radius: {{ border.radius }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>

# Button

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.btn</td><td class="result">the base button class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.btn-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        {% if item.name != 'transparent' %}
          <tr><td class="class">.btn-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td></tr>
        {% endif %}
      {% endfor %}
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.btn-outline-{{ item.name }}</td><td class="css">border-color: {{ item.color }}; text-color: {{ item.color }}; background-color: transparent;</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        {% if item.name != 'transparent' %}
          <tr><td class="class">.btn-outline-{{ item.name }}</td><td class="css">border-color: {{ item.color }}; text-color: {{ item.color }}; background-color: transparent;</td></tr>
        {% endif %}
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Buttons are **ONLY** to be used with an anchor `<a>` tag. The there are classes for all the theme and palette colors, so you can use `btn-primary` as well as `btn-blue-300`.

```html
<a class="btn btn-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-secondary" href="https://bootstrapemail.com">Secondary</a>
<a class="btn btn-success" href="https://bootstrapemail.com">Success</a>
<a class="btn btn-danger" href="https://bootstrapemail.com">Danger</a>
<a class="btn btn-warning" href="https://bootstrapemail.com">Warning</a>
<a class="btn btn-info" href="https://bootstrapemail.com">Info</a>
<a class="btn btn-light" href="https://bootstrapemail.com">Light</a>
<a class="btn btn-dark" href="https://bootstrapemail.com">Dark</a>
```

<a href="#" class="btn btn-primary">Primary</a>
<a href="#" class="btn btn-secondary">Secondary</a>
<a href="#" class="btn btn-success">Success</a>
<a href="#" class="btn btn-danger">Danger</a>
<a href="#" class="btn btn-warning">Warning</a>
<a href="#" class="btn btn-info">Info</a>
<a href="#" class="btn btn-light">Light</a>
<a href="#" class="btn btn-dark">Dark</a>

<div class="alert alert-warning">
  <strong>Warning:</strong> You must supply a url in the href. Using just pound sign is not enough for some emails to render an anchor tag correctly.
</div>

{% include header.html name="Usage" hr="false" %}
You can use *outlined* versions of every button by simply adding the `outline` keyword to the class like `btn-outline-primary` or `btn-outline-green-500`.

```html
<a class="btn btn-outline-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-outline-green-500" href="https://bootstrapemail.com">Green</a>
```
<a class="btn btn-outline-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-outline-success" href="https://bootstrapemail.com">Green</a>

{% include header.html name="Sizes" hr="true" %}
You can use `btn-sm` or `btn-lg` for smaller or larger buttons and text respectively. If you want to just adjust the padding size of a button you can use the [Padding](/docs/padding) utility classes.
```html
<a class="btn btn-primary btn-sm" href="https://bootstrapemail.com">Large button</a>
<a class="btn btn-primary btn-lg" href="https://bootstrapemail.com">Large button</a>
```

<a class="btn btn-primary btn-sm" href="https://bootstrapemail.com">Large button</a>
<a class="btn btn-primary btn-lg" href="https://bootstrapemail.com">Large button</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary" href="https://example.com">Click Me</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="https://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Click Me</a>
      </td>
    </tr>
  </tbody>
</table>
```

# Card

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.card</td><td class="css">background-color: white; border: 1px solid #e2e8f0; border-radius: 6px;</td></tr>
      <tr><td class="class">.card-body</td><td class="css">padding: 20px;</td></tr>
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Use to wrap content in a solid gray bordered container with rounded corners. Works well sitting on top of an email body with a `.bg-light` class and inside of a `.container`.

By default `.card` has no padding, you can use a card with or without a `.card-body`. Just like in Bootstrap a `.card-body` is just used to give `20px` padding to the card, you can also use a [padding](/docs/padding) utility to customize padding.

```html
<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>
```

<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="card">
  <div class="card-body">
    Some quick example text to build on the card title and make up the bulk of the card's content.
  </div>
</div>

```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="card" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important; width: 100%; overflow: hidden; border: 1px solid #e2e8f0;" bgcolor="#ffffff">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#ffffff">
        <table class="card-body" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
          <tbody>
            <tr>
              <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0; padding: 20px;" align="left">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
  </tbody>
</table>
```

# Configure 

{% include header.html name="Config" hr="false" %}
Configure different aspects of Bootstrap Email. It will look for a file in the working directory for `bootstrap_email.config.rb`. If you are using Rails, put this file in `config/initializers/bootstrap_email.rb`. Here is a list of the config options that you can customize.
```ruby
BootstrapEmail.configure do |config|
  # Defaults to ./bootstrap-email.scss or ./app/assets/stylesheets/bootstrap-email.scss in rails
  config.sass_email_location = File.expand_path('path/to/bootstrap-email.scss', __dir__)
  # Defaults to ./bootstrap-head.scss or ./app/assets/stylesheets/bootstrap-head.scss in rails
  config.sass_head_location = File.expand_path('path/to/bootstrap-head.scss', __dir__)
  # Custom sass that can be passed in to customize sass variables and such for the email sass
  config.sass_email_string = '// Pass in custom sass'
  # Custom sass that can be passed in to customize sass variables and such for the head sass
  config.sass_head_string = '// Pass in head custom sass'
  # Array of folders to add to the SASS load path to support imports in the custom SASS files
  config.sass_load_paths = [File.expand_path('some/folder', __dir__)]
  # Defaults to ./.sass-cache or ./tmp/cache/bootstrap-email/.sass-cache in rails
  config.sass_cache_location = [File.expand_path('some/folder', __dir__)]
  # Defaults to true, is disabled during CLI commands that output to standard out
  config.sass_log_enabled = true
  # Turn on or off whether or not rails will also include a plain text email part, Default: true
  config.generate_rails_text_part
end
```

{% include header.html name="Config Path" hr="true" %}
If you want to provide a path to a config file, you can use the `options: {config_path: 'path'}}` option in the `BootstrapEmail::Compiler.new()` method or with the `-c` flag via the CLI.
- Using the CLI:
```bash
bootstrap-email -c path/to/bootstrap-email.config.rb
```
- Using Ruby:
```ruby
html = '<div>Hello</div>'
path = File.expand_path('path/to/bootstrap-email.config.rb', __dir__)
BootstrapEmail::Compiler.new(html, options: {config_path: path}).perform_full_compile
```
Also any config above, `sass_email_location` for example, can be passed in via the `options` hash.

{% include header.html name="Customize Sass" hr="true" %}
If you want to customize styles like colors or spacing or even want to add custom styles to be compiled with the SCSS and inlined into your email you can use a config file. By default Bootstrap Email will look for a `bootstrap-email.scss` file in the root of the working directory / project.

Here are the 3 files of SASS variables that you can customize by overriding:
1. [General Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_variables.scss)
2. [Color Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_colors.scss)
2. [Utility Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_utilities.scss)

This is what a basic config file should contain:
```scss
//= @import bootstrap-email;
```

 This allows you to customize all you want surrounding the base SCSS that gets pulled in. Here is an example of setting different colors to be used:
```scss
// Override all colors to black
$primary: #000000;
$secondary: #000000;
$success: #000000;
$info: #000000;
$warning: #000000;
$danger: #000000;
$light: #000000;
$dark: #000000;

//= @import bootstrap-email;

// Make all links pink
a {
  color: pink;
}
```
For more examples of variables that can be overridden check out the SCSS files for [colors](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_colors.scss), [utilities](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_utilities.scss), and [variables](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_variables.scss)

{% include header.html name="Additional Methods" hr="true" %}

`BootstrapEmail.reset_config!` to reset all the configuration.

`BootstrapEmail.clear_sass_cache!` to clear the cached sass files.

# Container

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.container</td><td class="result">center aligned, max width 600px, left and right padding</td></tr>
      <tr><td class="class">.container-fluid</td><td class="result">full width, left and right padding</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Using the `container` class is the most common default email structure recommended. It should be used to wrap your entire pages contents. It has a 600px max-width which is standard for broad email support. It will be responsive on mobile devices.

```html
<div class="container">
  <!-- Content here -->
</div>
```

A `container-fluid` is unlike a container in that it doesn't have it's max-width set. It does however still have padding on the edges to give the content better spacing towards the edge of the email.

```html
<div class="container-fluid">
  <!-- Content here -->
</div>
```

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="container">
  <!-- Content here -->
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="container" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
  <tbody>
    <tr>
      <td align="center" style="line-height: 24px; font-size: 16px; margin: 0; padding: 0 16px;">
        <!--[if (gte mso 9)|(IE)]>
          <table align="center" role="presentation">
            <tbody>
              <tr>
                <td width="600">
        <![endif]-->
        <table align="center" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; max-width: 600px; margin: 0 auto;">
          <tbody>
            <tr>
              <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
                <!-- Content here -->
              </td>
            </tr>
          </tbody>
        </table>
        <!--[if (gte mso 9)|(IE)]>
                </td>
              </tr>
            </tbody>
          </table>
        <![endif]-->
      </td>
    </tr>
  </tbody>
</table>
```

# Display

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      {% for display in site.data.displays %}
        <tr><td class="class">.d-{{ display }}</td><td class="css">display: {{ display }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<p class="text-muted">Looking for flexbox support? Check out <a href="/docs/stack">stack documentation</a> for flexbox-like support in email using tables.</p>

{% include header.html name="Responsive" hr="false" %}
Here is an example of using the display utility to show and hide an element on mobile and hidden on desktop and vice versus.
```html
<span class="d-lg-none">Hidden on Desktop</span>
<span class="d-none d-lg-inline">Hidden on Mobile</span>
```

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="d-lg-none">Hidden on Desktop</span>
<span class="d-none d-lg-inline">Hidden on Mobile</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<!-- The desktop styles are inlined and overridden by a media query in the <head> of the document -->
<span class="d-lg-none" style="display: none;">Hidden on Desktop</span>
<span class="d-none d-lg-inline" style="display: inline;">Hidden on Mobile</span>
```

# Font Weight

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for weight in site.data.font_weights %}
        <tr><td class="class">.fw-{{ weight }}</td><td class="css">font-weight: {{ weight }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the weight of font.
```html
<p class="fw-100">Font weight 100</p>
<p class="fw-200">Font weight 200</p>
<p class="fw-300">Font weight 300</p>
<p class="fw-400">Font weight 400</p>
<p class="fw-500">Font weight 500</p>
<p class="fw-600">Font weight 600</p>
<p class="fw-700">Font weight 700</p>
<p class="fw-800">Font weight 800</p>
<p class="fw-900">Font weight 900</p>
```
<p style="font-weight: 100;">Font weight 100</p>
<p style="font-weight: 200;">Font weight 200</p>
<p style="font-weight: 300;">Font weight 300</p>
<p style="font-weight: 400;">Font weight 400</p>
<p style="font-weight: 500;">Font weight 500</p>
<p style="font-weight: 600;">Font weight 600</p>
<p style="font-weight: 700;">Font weight 700</p>
<p style="font-weight: 800;">Font weight 800</p>
<p style="font-weight: 900;">Font weight 900</p>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<p class="fw-100">Font weight 100</p>
<p class="fw-200">Font weight 200</p>
<p class="fw-300">Font weight 300</p>
<p class="fw-400">Font weight 400</p>
<p class="fw-500">Font weight 500</p>
<p class="fw-600">Font weight 600</p>
<p class="fw-700">Font weight 700</p>
<p class="fw-800">Font weight 800</p>
<p class="fw-900">Font weight 900</p>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<p class="fw-100" style="line-height: 24px; font-size: 16px; font-weight: 100 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-200" style="line-height: 24px; font-size: 16px; font-weight: 200 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-300" style="line-height: 24px; font-size: 16px; font-weight: 300 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-400" style="line-height: 24px; font-size: 16px; font-weight: 400 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-500" style="line-height: 24px; font-size: 16px; font-weight: 500 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-600" style="line-height: 24px; font-size: 16px; font-weight: 600 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-700" style="line-height: 24px; font-size: 16px; font-weight: 700 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-800" style="line-height: 24px; font-size: 16px; font-weight: 800 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-900" style="line-height: 24px; font-size: 16px; font-weight: 900 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
```

# Gap

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-{{ size }}</td><td class="result">{{ size | times: 4 }}px gap on all sides</td></tr>
      {% endfor %}
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-x-{{ size }}</td><td class="result">{{ size | times: 4 }}px horizontal gap</td></tr>
      {% endfor %}
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-y-{{ size }}</td><td class="result">{{ size | times: 4 }}px vertical gap</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Just like the margin and padding classes, multiply the class number by 4px to get the size. Ex. gap-10 is 40px.

{% include header.html name="Grid" hr="true" %}
By default the grid `.row` class has `24px` horizontal gutters. You can apply these gap classes to the row class to change horizontal and vertical gutters `row gap-4` will add `16px` gutters on all sizes. Top and bottom gutters are useful for when a grid is responsive and stacks columns vertically on mobile. [More about using Gap with Grid](/docs/grid#gap)

{% include header.html name="Stack" hr="true" %}
Use gap here to spread elements in a stack, horizontally if it is a `stack-x` and vertically if it is a `stack-y`. [More about using Gap with Stacks](/docs/grid#gap)

# Grid

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.row</td><td class="result">parent element to build a grid</td></tr>
      {% for item in site.data.grid_cols %}
        <tr><td class="class">.col-{{ item.name }}</td><td class="css">width: {{ item.width }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Grids work just like they do in Bootstrap, based on a 12 column grid. Make a row and give it columns. By default the grid holds it's structure on every device. It has a default horizontal gutter between elements of `24px`.

```html
<div class="row">
  <div class="col-3">.col-3</div>
  <div class="col-4">.col-4</div>
  <div class="col-5">.col-5</div>
</div>
```

<div class="row mb-4">
  <div class="col-3"><div class="border">.col-3</div></div>
  <div class="col-4"><div class="border">.col-4</div></div>
  <div class="col-5"><div class="border">.col-5</div></div>
</div>

{% include header.html name="Responsive" hr="true" %}
You can use the responsive <code>lg</code> modifier to make the grid snap back to vertical stacking on smaller devices.

```html
<div class="row">
  <div class="col-lg-3">.col-3</div>
  <div class="col-lg-4">.col-4</div>
  <div class="col-lg-5">.col-5</div>
</div>
```

{% include header.html name="Gap" hr="true" %}
To customize horizontal and vertical gutters see the [Gap Docs](/docs/gap) for more details. For example `row gap-0` would remove the gap between cells. In the example below, the `gap-12` adds a `48px` gap between all cells. The default gap between cells is `24px`.

```html
<div class="row gap-12">
  <div class="col-3">.col-3</div>
  <div class="col-4">.col-4</div>
  <div class="col-5">.col-5</div>
</div>
```

<div class="row g-5">
  <div class="col-lg-3"><div class="border">.col-3</div></div>
  <div class="col-lg-4"><div class="border">.col-4</div></div>
  <div class="col-lg-5"><div class="border">.col-5</div></div>
</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="row">
  <div class="col-3">This is a 1/4 of the row</div>
  <div class="col-3">This is a 1/4 of the row</div>
  <div class="col-6">This is a 1/2 of the row</div>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="row" role="presentation" border="0" cellpadding="0" cellspacing="0" style="table-layout: fixed; width: 100%;" width="100%">
  <tbody>
    <tr>
      <td class="col-3" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 25%; margin: 0;" align="left" valign="top">
        This is a 1/4 of the row
      </td>
      <td class="col-3" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 25%; margin: 0;" align="left" valign="top">
        This is a 1/4 of the row
      </td>
      <td class="col-6" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 50%; margin: 0;" align="left" valign="top">
        This is a 1/2 of the row
      </td>
    </tr>
  </tbody>
</table>
```

# Height

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.h-full</td><td class="css">height: 100%;</td></tr>
      <tr><td class="class">.h-auto</td><td class="css">height: auto</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.h-{{ size }}</td><td class="css">height: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td class="class">.max-h-full</td><td class="css">max-height: 100%;</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.max-h-{{ size }}</td><td class="css">max-height: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Like the [padding utilities](/docs/padding) it uses `4px` as the increment size for each number. So `h-10` is `10 * 4px` which is `40px`. To do 100% height you can use `h-full`. These height and max-height utilities are really useful for images because **images need a width and/or a height** for them to be rendered properly in many versions of Outlook.
```html
<img src="#" class="max-h-12 h-full" /> /* image 48px width */
<img src="#" class="max-h-150 h-full" /> /* image 600px width, use this for an image that is "full width" in a container in an email */
```

In combination with the [width](/docs/width) utilities you can do things like make a circle with number in it.
```html
<div class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle">1</div>
```
<div class="rounded-pill bg-primary text-white d-flex justify-content-center align-items-center" style="width: 40px; height: 40px;"><span>1</span></div>


{% include header.html name="Responsive" hr="true" %}
By default these classes target all devices. However if you just wanted to target desktop you could do `.h-lg-4`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a 40px height centered button on desktop. That would look like this:
```html
<a class="h-full h-lg-10 align-center btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle">1</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle w-full" role="presentation" style="border-radius: 9999px; color: #ffffff; width: 40px; height: 40px; text-align: center !important; vertical-align: middle !important;" bgcolor="#0d6efd" width="40" height="40">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 9999px; color: #ffffff; width: 40px; height: 40px; margin: 0;" align="center" bgcolor="#0d6efd" valign="middle" width="40" height="40">
        1
      </td>
    </tr>
  </tbody>
</table>
```

# HR

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">&lt;hr&gt;</td><td class="result">gray horizontal rule full width</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Add a horizontal rule to separate content. A consistent one that works and looks good in all email clients. By default it has top and bottom spacing of 20px, to use different top and bottom margin us a [margin](/docs/margin) utility class.

```html
<hr>
Hello
<hr class="my-0"> <!-- no top or bottom margin -->
```
<hr>
Hello
<hr class="my-0"> <!-- no top or bottom margin -->

{% include header.html name="Compiled Example" hr="false" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<hr>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="s-5 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 20px; font-size: 20px; width: 100%; height: 20px; margin: 0;" align="left" width="100%" height="20">
         
      </td>
    </tr>
  </tbody>
</table>
<table class="hr" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-top-width: 1px; border-top-color: #e2e8f0; border-top-style: solid; height: 1px; width: 100%; margin: 0;" align="left">
      </td>
    </tr>
  </tbody>
</table>
<table class="s-5 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 20px; font-size: 20px; width: 100%; height: 20px; margin: 0;" align="left" width="100%" height="20">
         
      </td>
    </tr>
  </tbody>
</table>
```

# Image

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.img-fluid</td><td class="css">
        height: auto;<br>
        max-width: 100%;<br>
        width: 100%;
      </td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Images can be very complicated in emails. Luckily Bootstrap email makes it easy. Images need to have at least either a width or a height for them to render properly in something like Outlook. To keep an element full width of it's container, give it the `img-fluid`. Doing so will set properties like the `width="100%"` attribute on the img tag which is required for Outlook rendering.

```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" />
```

For doing something other than 100% image with, use the sizing width and height utility classes with your images: [Width Docs](/docs/width) & [Height Docs](/docs/height).

{% include header.html name="Accessibility" hr="true" %}
Make sure you include a descriptive `alt` property on every image, not only does this help with accessibility but it's not uncommon for images to be blocked in an email client and this helps user see what image is being blocked. [More on alt tags](https://moz.com/learn/seo/alt-text)

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" />
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" style="height: auto; line-height: 100%; outline: none; text-decoration: none; display: block; max-width: 100%; width: 100%; border: 0 none;" width="100%">
```

# Line Height

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for size in site.data.line_heights %}
        <tr><td class="class">.lh-{{ size.name }}</td><td class="css">line-height: {{ size.size }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```

<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<p class="lh-1" style="line-height: 1; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm" style="line-height: 1.25; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base" style="line-height: 1.5; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg" style="line-height: 2; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```

# Margin

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.my-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer above and below</td></tr>
        <tr><td class="class">.mt-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer above</td></tr>
        <tr><td class="class">.mb-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer below</td></tr>
      {% endfor %}
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.s-{{ spacing }}</td><td class="result">Make a spacer {{ spacing | times: 4 }}px tall</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
Note: Margin is only supported on the top and bottom.

{% include header.html name="Margin Usage" hr="false" %}
There are two types of spacing Bootstrap Email supports. [Padding](/docs/padding) (applied to the inside of table cells) and [Margin](/docs/margin) (in the form of vertical spacers which are used to take up space between elements vertically).

Margin is very inconsistently supported in email clients. Instead of using `margin` in css the margin classes create spacers above and/or below and element for simpler syntax like Bootstrap. This example adds a spacer of 12px above and below the middle card. See [space between](/docs/space-between) for more info on adding spacers between elements.
```html
<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin above and below)</div>
<div class="card card-body">Bottom Card</div>
```

<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin about and below)</div>
<div class="card card-body">Bottom Card</div>

{% include header.html name="Spacer Usage" hr="true" %}
```html
<div class="s-3"></div>
```
Spacers hold not content, they are just put into the document to sit between elements in a vertical flow.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary my-3" href="http://example.com">Button with mega margin</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
         
      </td>
    </tr>
  </tbody>
</table>
<table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Button with mega margin</a>
      </td>
    </tr>
  </tbody>
</table>
<table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
         
      </td>
    </tr>
  </tbody>
</table>
```

# Padding


<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.p-{{ spacing }}</td><td class="css">padding: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.px-{{ spacing }}</td><td class="css">padding-left: {{ spacing | times: 4 }}px; padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.py-{{ spacing }}</td><td class="css">padding-top: {{ spacing | times: 4 }}px; padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pt-{{ spacing }}</td><td class="css">padding-top: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pr-{{ spacing }}</td><td class="css">padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pb-{{ spacing }}</td><td class="css">padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pl-{{ spacing }}</td><td class="css">padding-left: {{ spacing | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
There are two types of spacing Bootstrap Email supports. Padding (applied to the inside of table cells) and [Margin](/docs/margin) (in the form of vertical spacers which are used to take up space between elements vertically).
```html
<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>
```

<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary p-5" href="http://example.com">Button with mega padding</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="btn btn-primary p-5" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 20px; border: 1px solid #0d6efd;">Button with mega padding</a>
      </td>
    </tr>
  </tbody>
</table>
```

# Preview Text

<a class="anchor" name="reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Tag</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">&lt;preview&gt;</td><td class="result">custom element for adding preview text to emails</td></tr>
    </tbody>
  </table>
</div>

If you aren't familiar with preview text, it is the text that shows up in your inbox as a preview of the content inside the email. Here is more info about what it is and how it works on [Litmus.com](https://litmus.com/blog/the-ultimate-guide-to-preview-text-support)
<img class="d-block mx-auto w-50" src="/img/email-preview-text.png"/>

{% include header.html name="Usage" hr="true" %}
Bootstrap Email has a custom `<preview>` tag you can use to define preview text in your emails. This way it will show up as a preview of your email in your inbox but will be completely hidden when viewing the email itself.

```html
<preview>This text will show up as a preview but not in the email!</preview>
```

The message will also be padded with `&nbsp;` at the end of the message so that if you have a short preview text the contents of the email will not flow into the inbox preview.

Note: This element will be moved to just under the `<body>` tag when compiled. I would suggest keeping it in the top of your document for your sake but it can really be anywhere.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<preview>Act quick before the offer ends!</preview>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="preview" style="display: none; max-height: 0px; overflow: hidden;">
  Act quick before the offer ends&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</div>
```

# Responsive

This is a list of all the components that are responsive.
<ul>
  {% for page in site.pages %}
    {% if page.responsive == true %}
      <li>
        <a href="/docs/{{ page.title | downcase | replace: ' ', '-' }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>


When you see the
<span class="d-inline-block">
  <a href="/docs/themeable" class="badge m-0 d-flex align-items-center compatibility-badge">
    <span class="badge-check">
      <img src="/img/icons/check.svg" />
    </span>
    <span>Responsive</span>
  </a>
</span> badge it means the component has responsive breakpoints for different sized screens. The breakpoint is anything 600px or wider is considered `lg` and anything under 600px is `sm`. By default everything is "mobile first" which means the default class is both screen sizes.

A class that uses the `-lg` infix is only large devices. For example `w-full` is `width: 100%` on all screen sizes. But `w-full w-lg-10` is `width: 100%` on small screens and `width: 40px` on large screen sizes.

Note: Some email clients like Gmail mobile do not support any media queries and so some responsive functions do not work on them.

Not everything that is responsive uses these names. For example the `.container` is responsive by default and expands and contracts on different screens.

# Space Between

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.space-y-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer between every child element</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Similar to space between in [Tailwind](https://tailwindcss.com/docs/space), this allows you to space elements evenly vertically. Good for things like paragraphs of text. If you want horizontal spacing between elements or more complex alignment, check out the [Stack](/docs/stack) documentation.
```html
<div class="space-y-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>

```
<div>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
<div class="my-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
<div>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="space-y-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="space-y-3">
  <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
  <table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
    <tbody>
      <tr>
        <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
           
        </td>
      </tr>
    </tbody>
  </table>
    <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
  <table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
    <tbody>
      <tr>
        <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
           
        </td>
      </tr>
    </tbody>
  </table>
  <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
</div>
```

# Stack

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.stack-row</td><td class="result">generate a horizontals stack</td></tr>
      <tr><td class="class">.stack-col</td><td class="result">generate a vertical stack</td></tr>
      <tr><td class="class">.stack-ax-left</td><td class="css">text-align: left;</td></tr>
      <tr><td class="class">.stack-ax-center</td><td class="css">text-align: center;</td></tr>
      <tr><td class="class">.stack-ax-right</td><td class="css">text-align: right;</td></tr>
      <tr><td class="class">.stack-ay-top</td><td class="css">vertical-align: top;</td></tr>
      <tr><td class="class">.stack-ay-middle</td><td class="css">vertical-align: middle;</td></tr>
      <tr><td class="class">.stack-ay-bottom</td><td class="css">vertical-align: bottom;</td></tr>
      <tr><td class="class">.stack-ay-baseline</td><td class="css">vertical-align: baseline;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Stacks work similar to the way flexbox does to lay children elements out in a row or a column. To use a stack, all you need to do a wrap children elements in either a `stack-x` for row or a `stack-y` for a column.

```html
<div class="stack-row">
  <div>Lay a group of things</div>
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <div>Out horizontally</div>
</div>
```

<div class="d-flex">
  <div>Lay a group of things</div>
  <img style="width: 40px;" src="/img/icons/logo.png" />
  <div>Out horizontally</div>
</div>

{% include header.html name="Gap" hr="true" %}
Stacks are made really useful when combined with [Gaps](/docs/gap). Using a gap you can space a few icons out.

```html
<div class="stack-row gap-4">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-row gap-16">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
```

<div class="d-flex">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex">
  <img style="width: 40px; margin-right: 64px;" src="/img/icons/logo.png" />
  <img style="width: 40px; margin-right: 64px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>

{% include header.html name="Alignment" hr="true" %}
Stacks use HTMl tables to generate their layouts, that means we can use the power of table cells to align their contents horizontally and vertically. The classes `stack-ax-left`, `stack-ax-center`, and `stack-ax-right` center contents horizontally (**Note: you must either you an inline or inline-block child element for this to work as expected**). The classes `stack-ay-top`, `stack-ay-middle`, `stack-ay-bottom`, and `stack-ay-baseline` are for vertical alignment of child elements. By default everything defaults to top left alignment.

```html
<div class="stack-row gap-4">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-row gap-4 stack-ay-bottom">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-row gap-4 stack-ay-middle">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
```
<div class="d-flex align-items-start">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex align-items-end">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex align-items-center">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="stack-row gap-10">
  <div>stack item 1</div>
  <div>stack item 2</div>
  <div>stack item 3</div>
  <div>stack item 4</div>
  <div>stack item 5</div>
  <div>stack item 6</div>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="stack-row gap-10" role="presentation" border="0" cellpadding="0" cellspacing="0">
  <tbody>
    <tr>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 1</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 2</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 3</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 4</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 5</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 0; margin: 0;" align="left" valign="top">
        <div>stack item 6</div>
      </td>
    </tr>
  </tbody>
</table>
```

# Table

<a class="anchor" name="reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.table</td><td class="result">applies the basic styles for a table, required for use with classes below</td></tr>
      <tr><td class="class">.table-bordered</td><td class="result">table with border on all size</td></tr>
      <tr><td class="class">.table-striped</td><td class="result">table with every other row striped</td></tr>
      <tr><td class="class">.thead-light</td><td class="result">light table header</td></tr>
      <tr><td class="class">.thead-dark</td><td class="result">dark table header</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.table-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
```html
<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>
```

<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>

{% include header.html name="Compiled Example" hr="true" %}

<span class="badge rounded-pill badge-input">Input</span>
```html
<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="table table-striped thead-default table-bordered" border="0" cellpadding="0" cellspacing="0" style="width: 100%; max-width: 100%; border: 1px solid #e2e8f0;">
  <thead>
    <tr>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 1</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 2</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 3</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr style="" bgcolor="#f2f2f2">
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
    <tr class="table-success" style="" bgcolor="#f2f2f2">
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 4</td>
    </tr>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
  </tbody>
</table>
```

# Text Align

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.text-left</td><td class="css">text-align: left;</td></tr>
      <tr><td class="class">.text-right</td><td class="css">text-align: right;</td></tr>
      <tr><td class="class">.text-center</td><td class="css">text-align: center;</td></tr>
      <tr><td class="class">.text-justify</td><td class="css">text-align: justify;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<div class="text-left">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-right">This text is to the right</div>
<div class="text-justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```

<div class="text-start">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-end">This text is to the right</div>
<div style="text-align: justify;">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="text-left">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-right">This text is to the right</div>
<div class="text-justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="text-left" style="" align="left">This text is to the left</div>
<div class="text-center" style="" align="center">This text is to the center</div>
<div class="text-right" style="" align="right">This text is to the right</div>
<div class="text-justify" style="" align="justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```

# Text Color 

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.text-{{ item.name }}</td><td class="css">color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.text-{{ item.name }}</td><td class="css">color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-green-500">Green 500 Text color</span>
<span class="text-yellow-500">Yellow 500 Text color</span>
```

<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-success">Green 500 Text color</span>
<span class="text-warning">Yellow 500 Text color</span>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-green-500">Green 500 Text color</span>
<span class="text-yellow-500">Yellow 500 Text color</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<span class="text-primary" style="color: #0d6efd;">Primary Text color</span>
<span class="text-muted" style="color: #718096;">Muted Text color</span>
<span class="text-danger" style="color: #dc3545;">Danger Text color</span>
<span class="text-green-500" style="color: #198754;">Green 500 Text color</span>
<span class="text-yellow-500" style="color: #ffc107;">Yellow 500 Text color</span>
```

# Text Size

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for size in site.data.font_sizes %}
        <tr><td class="class">.text-{{ size.name }}</td><td class="css">font-size: {{ size.size }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
These utility classes are good for more fine tuned adjustments of font size.
```html
<p class="text-xs">Text size xs</p>
<p class="text-sm">Text size sm</p>
<p class="text-base">Text size base</p>
<p class="text-lg">Text size lg</p>
<p class="text-xl">Text size xl</p>
<p class="text-2xl">Text size 2xl</p>
<p class="text-3xl">Text size 3xl</p>
<p class="text-4xl">Text size 4xl</p>
<p class="text-5xl">Text size 5xl</p>
<p class="text-6xl">Text size 6xl</p>
<p class="text-7xl">Text size 7xl</p>
```
{% for size in site.data.font_sizes %}
  <p style="font-size: {{ size.size }};">Text size {{ size.name }}</p>
{% endfor %}

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="text-xs">Text size xs</span>
<span class="text-sm">Text size sm</span>
<span class="text-base">Text size base</span>
<span class="text-lg">Text size lg</span>
<span class="text-xl">Text size xl</span>
<span class="text-2xl">Text size 2xl</span>
<span class="text-3xl">Text size 3xl</span>
<span class="text-4xl">Text size 4xl</span>
<span class="text-5xl">Text size 5xl</span>
<span class="text-6xl">Text size 6xl</span>
<span class="text-7xl">Text size 7xl</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<span class="text-xs" style="font-size: 12px; line-height: 14.4px;">Text size xs</span>
<span class="text-sm" style="font-size: 14px; line-height: 16.8px;">Text size sm</span>
<span class="text-base" style="font-size: 16px; line-height: 19.2px;">Text size base</span>
<span class="text-lg" style="font-size: 18px; line-height: 21.6px;">Text size lg</span>
<span class="text-xl" style="font-size: 20px; line-height: 24px;">Text size xl</span>
<span class="text-2xl" style="font-size: 24px; line-height: 28.8px;">Text size 2xl</span>
<span class="text-3xl" style="font-size: 30px; line-height: 36px;">Text size 3xl</span>
<span class="text-4xl" style="font-size: 36px; line-height: 43.2px;">Text size 4xl</span>
<span class="text-5xl" style="font-size: 48px; line-height: 57.6px;">Text size 5xl</span>
<span class="text-6xl" style="font-size: 64px; line-height: 76.8px;">Text size 6xl</span>
<span class="text-7xl" style="font-size: 80px; line-height: 96px;">Text size 7xl</span>
```

# Themable

When you see the
<span class="d-inline-block">
  <a href="/docs/themeable" class="badge m-0 d-flex align-items-center compatibility-badge">
    <span class="badge-check">
      <img src="/img/icons/check.svg" />
    </span>
    <span>Themeable</span>
  </a>
</span> badge it means the component has the following classes that you can use color the component. Just like Bootstrap, the convention is `{component}-{theme-color}`.

```html
{component}-primary
{component}-secondary
{component}-success
{component}-danger
{component}-warning
{component}-info
{component}-light
{component}-dark
```

Bootstrap Email uses the same default color scheme that Bootstrap 4 does.
<div class="themable-example text-white bg-primary">primary</div>
<div class="themable-example text-white bg-secondary">secondary</div>
<div class="themable-example text-white bg-success">success</div>
<div class="themable-example text-white bg-danger">danger</div>
<div class="themable-example bg-warning">warning</div>
<div class="themable-example text-white bg-info">info</div>
<div class="themable-example bg-light">light</div>
<div class="themable-example text-white bg-dark">dark</div>

<style>
  .themable-example{
    width: 100px;
    height: 100px;
    border-radius: 10px;
    display: inline-block;
    margin: 0 1rem 1rem 0;
    padding: 2.25rem 0;
    text-align: center;
  }
</style>

#### Customize Theme

Bootstrap Email makes is really easy to customize the theme colors. You can override each color in your sass file before the `bootstrap-email` import:
```scss
$theme-primary: #007bff;
$theme-secondary: #868e96;
$theme-success: #28a745;
$theme-danger: #dc3545;
$theme-warning: #ffc107;
$theme-info: #17a2b8;
$theme-light: #f8f9fa;
$theme-dark: #343a40;

@import 'bootstrap-email';
```

Note: These are the current defaults for the theme colors.

# Typography

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">&lt;h1&gt;, .h1</td><td class="css">font-size: 36px;</td></tr>
      <tr><td class="class">&lt;h2&gt;, .h2</td><td class="css">font-size: 32px;</td></tr>
      <tr><td class="class">&lt;h3&gt;, .h3</td><td class="css">font-size: 28px;</td></tr>
      <tr><td class="class">&lt;h4&gt;, .h4</td><td class="css">font-size: 24px;</td></tr>
      <tr><td class="class">&lt;h5&gt;, .h5</td><td class="css">font-size: 20px;</td></tr>
      <tr><td class="class">&lt;h6&gt;, .h6</td><td class="css">font-size: 16px;</td></tr>
      <tr><td class="class">&lt;strong&gt;</td><td class="css">font-weight: bold;</td></tr>
      <tr><td class="class">&lt;em&gt;</td><td class="css">font-style: italic;</td></tr>
      <tr><td class="class">.underline, &lt;u&gt;</td><td class="css">text-decoration: underline;</td></tr>
      <tr><td class="class">.no-underline</td><td class="css">text-decoration: none;</td></tr>
      <tr><td class="class">.line-through, &lt;s&gt;</td><td class="css">text-decoration: line-through;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Many basic typography options. If you want more text control check out [Text Align](/docs/text-align), [Text Color](/docs/text-color), [Text Size](/docs/text-size), [Font Weight](/docs/font-weight), and [Line Height](/docs/line-height).
```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>
<div class="h1">any tag as h1</div>
<div class="h2">any tag as h2</div>
<div class="h3">any tag as h3</div>
<div class="h4">any tag as h4</div>
<div class="h5">any tag as h5</div>
<div class="h6">any tag as h6</div>
<h1 class="display-1">Display 1</h1>
<h1 class="display-2">Display 2</h1>
<h1 class="display-3">Display 3</h1>
<h1 class="display-4">Display 4</h1>
<h1 class="display-5">Display 5</h1>
<h1 class="display-6">Display 6</h1>
<strong>bold text</strong>
<u>underlined text</u>
<em>italicized text</em>
<s>strike through text</s>
```

# h1
## h2
### h3
#### h4
##### h5
###### h6
# any tag as h1
## any tag as h2
### any tag as h3
#### any tag as h4
##### any tag as h5
###### any tag as h6
<strong>bold text</strong>
<u>underlined text</u>
<em>italicized text</em>
<s>strike through text</s>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<h1>This is an h1</h1>
<h2>This is an h2</h2>
<h3>This is an h3</h3>
<h4>This is an h4</h4>
<h5>This is an h5</h5>
<h6>This is an h6</h6>
<strong>Bold Text</strong>
<strong>Bold Text</strong>
<u>Underlined Text</u>
<em>Italic Text</em>
<s>Strike Through Text</s>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<h1 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 36px; line-height: 43.2px; margin: 0;" align="left">This is an h1</h1>
<h2 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 32px; line-height: 38.4px; margin: 0;" align="left">This is an h2</h2>
<h3 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 28px; line-height: 33.6px; margin: 0;" align="left">This is an h3</h3>
<h4 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 24px; line-height: 28.8px; margin: 0;" align="left">This is an h4</h4>
<h5 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 20px; line-height: 24px; margin: 0;" align="left">This is an h5</h5>
<h6 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 16px; line-height: 19.2px; margin: 0;" align="left">This is an h6</h6>
<strong>Bold Text</strong>
<strong>Bold Text</strong>
<u>Underlined Text</u>
<em>Italic Text</em>
<s>Strike Through Text</s>
```

# Usage

#### Environment Support
- [Command Line](#command-line)
- [Ruby](#ruby)
- [Ruby on Rails](#ruby-on-rails)
- [Online editor](#online-editor)

{% include header.html name="Command Line" hr="false" %}

[Ruby](https://www.ruby-lang.org/en/documentation/installation/) is required to be installed on the machine you are using to run Bootstrap Email.

1: Install bootstrap email via [Ruby Gems](https://rubygems.org/gems/bootstrap-email)
```bash
gem install bootstrap-email
```

2: There are many ways to use the command line to compile emails:
```bash
# compile all files ending in .html in the current directory
bootstrap-email
# compile the file email.html and save it to the file out.html
bootstrap-email email.html > out.html
# compile a relative path to a file
bootstrap-email ./public/index.html
# specify a path pattern and a destination directory for compiled emails to be saved to
bootstrap-email -p 'emails/*' -d 'emails/compiled/*'
# compile for a string
bootstrap-email -s '<a href="#" class="btn btn-primary">Some Button</a>'
# compile to plain text
bootstrap-email -t -s '<a href="#" class="btn btn-primary">Some Button</a>'
# pipe a file into bootstrap-email
cat input.html | bootstrap-email
# specify config path to use to customize things like colors
bootstrap-email -c bootstrap-email.scss
```

Help: run the command `bootstrap-email -h` for help on all options.

{% include header.html name="Ruby" hr="false" %}

1: Add Bootstrap Email to your `Gemfile`

```ruby
gem 'bootstrap-email'
```

2: Usage is simple, there are two ways to call Bootstrap Email, string and file.
```ruby
# Pass in any html string or html document as a string
html = '<a href="#" class="btn btn-primary">A button</a>'
BootstrapEmail::Compiler.new(html).perform_full_compile

# Pass in a full path to a file
file_path = File.expand_path('path/to/a/file.html', __dir__)
BootstrapEmail::Compiler.new(file_path, type: :file).perform_full_compile
```

{% include header.html name="Ruby on Rails" hr="false" %}

1: Add Bootstrap Email to your `Gemfile`

```ruby
gem 'bootstrap-email'
```

2: You need to create the mailer template which will wrap the email content. Create the file `/app/views/layouts/bootstrap-mailer.html.erb` and paste this HTML into it. (It is very similar to the default mailer).
```erb
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html lang="en">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="x-apple-disable-message-reformatting">
    <meta http-equiv="x-ua-compatible" content="ie=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="format-detection" content="telephone=no, date=no, address=no, email=no">
  </head>
  <body>
    <%= yield %>
  </body>
</html>
```

3: Specify the layout for the actions you want to build with bootstrap email. You can specify it for all with ApplicationMailer.
```ruby
class ApplicationMailer < ActionMailer::Base
  layout 'bootstrap-mailer'
end
```
Refer to the [official ActionMailer documentation](http://guides.rubyonrails.org/action_mailer_basics.html#action-mailer-layouts) on more info about using a different layout for different mailers.

<!-- 4: Create a new stylesheet `/app/assets/stylesheets/application-mailer.scss` and import `bootstrap-email`. This is where your custom styles and overrides that you want to be inlined should live.

```sass
@import 'bootstrap-email';
```

5: Add this line in `/config/initializers/asset.rb` to compile your new SASS file.

```ruby
Rails.application.config.assets.precompile += %w( application-mailer.scss )
```

6: Create the view file `/app/views/example_mailer/greet.html.erb`.

You can also create the view `/app/views/example_mailer/greet.text.erb`. In this case don't forget to create also the textual layout `/app/views/layouts/example_mailer.text.erb`.

If you do  not create a textual view file, a text part is automatically added by the `premailer-rails` gem. -->


4: That's it! Now all you need to do to use it instead of using the `mail()` method, you use the `bootstrap_mail()` method to kick off Bootstrap Email compilation!

```ruby
class ExampleMailer < ApplicationMailer
  def greet
    bootstrap_mail(
      to: 'to@example.com',
      from: 'from@example.com',
      subject: 'Hi From Bootstrap Email',
    )
  end
end
```

You can also use the `format` in the usual way.
```ruby
class ExampleMailer < ApplicationMailer
  def greet
    bootstrap_mail(
      to: 'to@example.com',
      from: 'from@example.com',
      subject: 'Hi From Bootstrap Email',
      ) do |format|
        format.html { layout 'custom_bootstrap_layout' }
        format.text # here example_mailer.text.erb is used
      end
  end
end
```

{% include header.html name="Online editor" hr="false" %}
An easier, but less integrated and customizable way to use Bootstrap Email is the online editor.
- Write an email and test it's rendering quickly
- Test on desktop and mobile responsive device widths
- Save emails to your account to come back to
- Send test emails directly to your inbox

<a href="https://app.bootstrapemail.com/editor?version=1" class="btn btn-purple my-3">Try the Online Editor</a>
<img class="w-100" src="/img/editor.png" />

# Width

<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.w-full</td><td class="css">width: 100%;</td></tr>
      <tr><td class="class">.w-auto</td><td class="css">width: auto</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.w-{{ size }}</td><td class="css">width: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td class="class">.max-w-full</td><td class="css">max-width: 100%;</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.max-w-{{ size }}</td><td class="css">max-width: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Like the [padding utilities](/docs/padding) it uses `4px` as the increment size for each number. So `w-10` is `10 * 4px` which is `40px`. To do 100% width you can use `w-full`. These width and max-width utilities are really useful for images because **images need a width and/or a height** for them to be rendered properly in many versions of Outlook.
```html
<img src="#" class="max-w-12 w-full" /> /* image 48px width */
<img src="#" class="max-w-150 w-full" /> /* image 600px width, use this for an image that is "full width" in a container in an email */
```

{% include header.html name="Responsive" hr="true" %}
By default these classes target all devices. However if you just wanted to target desktop you could do `.w-lg-4`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a auto width centered button on desktop. That would look like this:
```html
<a class="w-full w-lg-auto align-center btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>
