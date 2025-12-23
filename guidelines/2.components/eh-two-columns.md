---
title: TwoColumns
description: Create a two columns in an instant and populate them with your own content, whatever it may be
constructorName: EhTwoColumns
layout: doc
---

### Usage

#### Presentation
The <b>{{ $doc.constructorName }}</b> constructor enables you to provide any content presented in two
columns and one row.
> Note: The `border` in `wrapper` is only for visual understanding of the <b>{{ $doc.constructorName }}</b> boundry. Component itself does not have that predefined

#### Example Basic (text)

::EhTwoColumns
---
ui: 
  wrapper: border
---
This text is displayed in the left column first row.

Text is displayed in the right column first row.

This text is displayed in the left column second row.

Text text is displayed in the right column second row.
::

The above example is written as:

```mdc 
::EhTwoColumns
---
ui: 
  wrapper: border
---
This text is displayed in the left column first row.

Text is displayed in the right column first row.

This text is displayed in the left column second row.

Text text is displayed in the right column second row.
::
```

#### Example Basic (text/image)
It is possible to add text or an image to one or to both columns. For example, text and image:

::EhTwoColumns
---
ui: 
  wrapper: shadow-2xl
---
This text should be in the left column. 

![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-full .rounded-2xl}
::

This is how the above example is written:

```mdc
::EhTwoColumns
This text should be in the left column. 

![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-full .rounded-2xl}
::
```
#### Example Basic (image/text)
The order of the elements determine the left and right column content.

::EhTwoColumns
---
ui: 
  wrapper: shadow-2xl
---
![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-full .rounded-2xl}

This text should be in the right column. 
::

This is how the above example is written:

```mdc
::EhTwoColumns
![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-full .rounded-2xl}

This text should be in the right column. 
::
```

### Props
The <b>{{ $doc.constructorName }}</b> constructor supports the following properties:

#### Properties and Attributes Description
The `gap` property controls gutters between columns.
Values for this property and its basic usage can be found in
[TailwindCSS](https://tailwindcss.com/docs/gap){target="_blank"} documentation.

<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Attribute</th>
      <th>Default</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2"><code>ui</code></td>
      <td>n/a</td>
      <td>n/a</td>
      <td>Optional configuration object for customizing various styling aspects of the <code>EhTwoColumns</code> component.</td>
    </tr>
    <tr>
      <td><code>wrapper</code></td>
      <td><code>config.wrapper</code></td>
      <td>Defines the overall styling for the container that holds all the elements inside of the <code>EhTwoColumns</code>. 
    </tr>
    <tr>
      <td><code>size</code></td>
      <td>n/a</td>
      <td><code>L</code></td>
      <td>
        Optional. Specifies the width of the left column.</br>
        <b>Options:</b> <code>2XS</code>, <code>XS</code>, <code>S</code>, <code>M</code>, <code>L</code>, <code>XL</code>, <code>2XL</code>, <code>3XL</code> & <code>4XL</code>
      </td>
    </tr>
    <tr>
      <td><code>gap</code></td>
      <td>n/a</td>
      <td><code>gap-4</code></td>
      <td>
        Optional. Controls the gutters between columns.</br>
        <b>Options:</b> Refer to the <a href="https://tailwindcss.com/docs/gap" target="_blank">Tailwind CSS documentation</a> for values and usage.</td>
    </tr>
    <td><code>description</code></td>
      <td>n/a</td>
      <td>n/a</td>
      <td>Intented to be used as a help to content writter. Doesn`t render on website.
    </td>
  </tbody>
</table>

#### Example Usage
##### Advanced Settings 
It is possible to nest other components inside of the <b>{{ $doc.constructorName }}</b> component as e.g., an `EhSegment` and nest a <b>{{ $doc.constructorName }}</b> component to provide special effects. For instance the following example contains:
* Two columns
  * **Column 1**: Contains an image with inline style.
  * **Cloumn 2**: It is a `EhSegment` with background color, shadow and other special styles which in turn contains:
    * Markdown text,
    * Bullet list,
    * <b>{{ $doc.constructorName }}</b> : A nested <b>{{ $doc.constructorName }}</b> module at the bottom of the second column which contains:
      * *Sub-Column 1*: A markdown text styled inline,
      * *Sub-Column 2*: An image that has been styled by rounding the corners.

::EhTwoColumns
---
ui: 
  wrapper: shadow-2xl
---
![laptop](https://free-images.com/tn/f4f3/coffee_apple_iphone_laptop.jpg){.not-prose .w-full .rounded-2xl .shadow-2xl}

:::EhSegment
---
ui:
  wrapper: bg-cyan-300 rounded-2xl border shadow-md p-1 # Comment
---
For more elaborated content in one of the columns it's better to utilize the `EhSegment` 
component.

This component enables more *Markdown* content to be added to the column. This content
can contain all available contractors as other parts of the *Markdown* document:

* lists, images, tables, links
* other components

It can contain nested <b>{{ $doc.constructorName }}</b> component as well, if that is needed for achieving
desired effect.
::EhTwoColumns
---
size: 2XL
---
[Let your creativity blosom]{.text-4xl .bg-gradient-to-r .from-blue-600 .to-orange-400 .bg-clip-text .text-transparent .inline-block}

![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-1/2 .rounded-full}
::

:::

::

This is how the above example is written in markdown:

```mdc
::EhTwoColumns
![laptop](https://free-images.com/tn/f4f3/coffee_apple_iphone_laptop.jpg){.not-prose .w-full .rounded-2xl .shadow-2xl}

:::EhSegment
---
ui:
  wrapper: bg-cyan-300 rounded-2xl border shadow-md p-1 # Comment
---
For more elaborated content in one of the columns it's better to utilize the `EhSegment` 
component.

This component enables more *Markdown* content to be added to the column. This content
can contain all available contractors as other parts of the *Markdown* document:

* lists, images, tables, links
* other components

It can contain nested <b>{{ $doc.constructorName }}</b> component as well, if that is needed for achieving
desired effect.
::EhTwoColumns
---
size: 2XL
---
[Let your creativity blosom]{.text-4xl .bg-gradient-to-r .from-blue-600 .to-orange-400 .bg-clip-text .text-transparent .inline-block}

![image](https://free-images.com/sm/3b8f/dalmatiner_schw_braun.jpg){.not-prose .w-1/2 .rounded-full}
::

:::

::
```

You can notice that in the right column, encoupsulated with `EhSegment`
component there is a <b>{{ $doc.constructorName }}</b> component with different withs of the
columns.

The relationship between sizes of two columns can be controled using the property `size`.
The values of this property are define in [T-shirt]{} sizes starting from '2XS' all the
way up to '4XL', see below. Default value of the `size` property is 'L'.

#### Two-Columns and Size
The image displayed below is composed of the following components:

* An `EhSegment` component that nests several <b>{{ $doc.constructorName }}</b> components, with one for each row. The <b>{{ $doc.constructorName }}</b> component uses the `size` attribute to define the width of the left column.
* Inside each <b>{{ $doc.constructorName }}</b> component, two `EhSegment` components are nested. These `EhSegment` components use the `wrapper` attribute to provide background color and text to define the size (left column) and proportion (right column). 

::EhSegment
---
ui:
  wrapper: grid grid-rows-1 gap-4
---
  ::EhTwoColumns
  ---
  size: 2XS
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    2XS
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    9/10
    :::
  ::

  ::EhTwoColumns
  ---
  size: XS
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    XS
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    4/5
    :::
  ::

  ::EhTwoColumns
  ---
  size: S
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    S
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    3/4
    :::
  ::

  ::EhTwoColumns
  ---
  size: M
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    M
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    2/3
    :::
  ::

  ::EhTwoColumns
  ---
  size: L
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    L
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    1/2
    :::
  ::

  ::EhTwoColumns
  ---
  size: XL
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    XL
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    1/3
    :::
  ::

  ::EhTwoColumns
  ---
  size: 2XL
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    2XL
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    1/4
    :::
  ::

  ::EhTwoColumns
  ---
  size: 3XL
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    3XL
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    1/5
    :::
  ::

  ::EhTwoColumns
  ---
  size: 4XL
  ---
    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-200 text-center dark:text-black
    ---
    4XL
    :::

    :::EhSegment
    ---
    ui:
      wrapper: bg-slate-300 text-center dark:text-black
    ---
    1/10
    :::
  ::
::

### Config
The style attributes can be modified via the property `ui` and are stored in the <code><b>{{ $doc.constructorName }}</b><b>.ts</b></code> file:

```ts
export default {
  wrapper: "",
  default: {
    size: "L",
    gap: "gap-4"
  }
}
```

#### Class Descriptions
These represent the class values utilized in the <b>{{ $doc.constructorName }}</b> constructor. These values are customizable and can be strengthened or overridden through the `ui` properties' attributes.

_**wrapper**_:

* **Value**: `""`
* **Description**: This defines the overall styling for the container. Currently, there are no styles applied to the wrapper.

_**default**_:

* **Value**: `{ size: "L", gap: "gap-4" }`
* **Description**: This object holds the default Tailwind CSS values that might be used as fallback or initial styles. In this case, it sets a default size value of "L" and a default gap value of "gap-4".

_**size**_:

* *Value*: `"L"`
* **Description**: This defines the default width of the left column. The value "L" indicates a large size.

_**gap**_:

* **Value**: `"gap-4"`
* **Description**: This defines the default gutter size between columns. The value "gap-4" applies a gap utility class from Tailwind CSS to add spacing between the columns. Detailed information about the gap property can be found in the Tailwind CSS documentation.

These style properties ensure that the <b>{{ $doc.constructorName }}</b> component is visually appealing and flexible, allowing for a wide range of customization to meet specific design requirements. This value only can be modified in the <code><b>{{ $doc.constructorName }}</b><b>.ts</b></code> file, it cannot be modified via markdown.
