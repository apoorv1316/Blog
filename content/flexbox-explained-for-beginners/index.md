---
title: "Flexbox explained for beginners"
description: "Flexbox also known as flexible box is a type of layout model in CSS that makes it super easy to design responsive layouts."
date: "2020-02-05T04:47:41.337Z"
categories: []
published: true
canonical_link: https://medium.com/@tiwari.apoorv1316/flexbox-explained-for-beginners-23859dcc87bc
redirect_from:
  - /flexbox-explained-for-beginners-23859dcc87bc
---

Flexbox also known as flexible box is a type of layout model in CSS that makes it super easy to design responsive layouts.

The whole idea behind the Flexbox layout model is to allow elements to be laid out in any direction, flex their size to either fill up unused space or shrink to avoid overflowing their parent element, either horizontally or vertically.

To truly be able to flex with Flexbox, we have to understand how it works.

Let’s break it down into its properties into two namely;

1.  Flex Container
2.  Flex Items

### Flex Container

This is the parent html element that houses the items you want to lay out.

To use any of the flex properties, this container has to be created.

It’s what creates the context that allows every other flex properties to work.

![Creating a flex container and flex items](./asset-1.png)

#### align-items

This allows you to align the items in the flex container vertically, regardless of the height of the item with respect to their flex container or each other.

The values it accepts are: **_flex-start_** | **_flex-end_** | **_center_** | **_baseline_** | **_stretch_**

`align-items: flex-start;`

The flexbox items are aligned at the **start** of the **cross axis**.

By default, the cross axis is vertical. This means the flexbox items will be aligned _vertically_ at the _top_.

![](./asset-2.png)

`align-items: flex-end;`

The flexbox items are aligned at the **end** of the **cross axis**.

By default, the cross axis is vertical. This means the flexbox items will be aligned _vertically_ at the _bottom_.

![](./asset-3.png)

`align-items: center;`

The flexbox items are aligned at the **center** of the **cross axis**.

By default, the cross axis is vertical. This means the flexbox items will be **centered** _vertically_.

![](./asset-4.png)

`align-items: baseline;`

The flexbox items are aligned at the **baseline** of the **cross axis**.

By default, the cross axis is vertical. This means the flexbox items will align themselves in order to have the _baseline_ of their _text_ align along a horizontal line.

![](./asset-5.png)

`align-items: stretch;`

The flexbox items will stretch across the whole **cross axis**.

By default, the cross axis is vertical. This means the flexbox items will fill up the whole vertical space.

![](./asset-6.png)

#### justify-content

This is the opposite of **align-items,** it aligns its item horizontally regardless of the width of the item with respect to their container or each other.

Values: **_flex-start_** | **_flex-end_** | **_center_** | **_space-between_** | **_space-around_** | **_space-evenly._**

`justify-content: flex-start;`

The flexbox/grid items are pushed towards the **start** of the container’s main axis.

![](./asset-7.png)

`justify-content: flex-end;`

The flexbox/grid items are pushed towards the **end** of the container’s main axis.

![](./asset-8.png)

`justify-content: center;`

The flexbox/grid items are **centered** along the container’s main axis.

![](./asset-9.png)

`justify-content: space-between;`

The remaining space is distributed **between** the flexbox/grid items.

![](./asset-10.png)

`justify-content: space-around;`

The remaining space is distributed **around** the flexbox/grid items: this adds space _before_ the first item and _after_ the last one.

![](./asset-11.png)

#### flex-wrap

The `flex-wrap` property specifies whether the flex items should break to the next line or not.

By default all flex items will try to fit in a single line, but this property tells the browser to break them into another line when they become way too many to fit in a single line.

This line we speak of is also known as a F**lex line**.

Values: **_nowrap_** | **_wrap_** | **_wrap-reverse_**

`flex-wrap: nowrap;`

The flexbox items will remain on a **single line**, no matter what, and will eventually overflow if needed.

![](./asset-12.png)

`flex-wrap: wrap;`

The flexbox items will be distributed among **multiple lines** if needed.

![](./asset-13.png)

`flex-wrap: wrap-reverse;`

The flexbox items will be distributed among **multiple lines** if needed. Any additional line will appear **before** the previous one.

![](./asset-14.png)

#### align-content

This property modifies the behavior of the **flex-wrap** property.

It essentially behaves like the **align-items** property, only that it aligns the flex lines instead of the flex items.

To make this property work, `flex-wrap: wrap` has to be set on the flex container and the flex lines have to be more than one.

Values: **_flex-start_** | **_flex-end_** | **_center_** | **_space-between_** | **_space-around_** | **_stretch_**

`align-content: stretch;`

Each line will stretch to _fill_ the remaining space.

In this case, the container is `300px` high. All boxes are `50px` high, apart from the second one who is `100px` high.

-   The first line is **100px** high
-   The second line is **50px** high
-   The remaining space is **150px**

This remaining space is distributed equally amongst the two lines:

-   The first line is now **175px** high
-   The second line is now **125px** high

![](./asset-15.png)

`align-content: flex-start;`

Each line will only fill the space it _needs_. They will all move towards the **start** of the flexbox/grid container’s cross axis.

![](./asset-16.png)

`align-content: flex-end;`

Each line will only fill the space it _needs_. They will all move towards the **end** of the flexbox/grid container’s cross axis.

![](./asset-17.png)

`align-content: center;`

Each line will only fill the space it _needs_. They will all move towards the **center** of the flexbox/grid container’s cross axis.

![](./asset-18.png)

`align-content: space-between;`

Each line will only fill the space it _needs_. The _remaining_ space will appear **between** the lines

![](./asset-19.png)

`align-content: space-around;`

Each line will only fill the space it _needs_. The _remaining_ space will be distributed equally **around** the lines: before the first line, between the two, and after the last one.

![](./asset-20.png)

#### flex-direction

This defines which direction the browser should stack the Flex items i.e vertically or horizontally.

Values: **_row_** | **_row-reverse_** | **_column_** | **_column-reverse_**

`flex-direction: row;`

The flexbox items are ordered the **same** way as the **text direction**, along the **main axis**.

![](./asset-21.png)

`flex-direction: row-reverse;`

The flexbox items are ordered the **opposite** way as the **text direction**, along the **main axis**.

![](./asset-22.png)

`flex-direction: column;`

The flexbox items are ordered the **same** way as the **text direction**, along the **cross axis**.

![](./asset-23.png)

`flex-direction: column-reverse;`

The flexbox items are ordered the **opposite** way as the **text direction**, along the **cross axis**.

![](./asset-24.png)

So these were the flex container properties and in the next part, we will cover properties of flex items.

**Happy Coding!**
