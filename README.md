# Tiny Css Class Generator
Utility classes help you work within the constraints of a system instead of littering your stylesheets with arbitrary values. They make it easy to be consistent with color choices, spacing, typography, shadows, and everything else that makes up a well-engineered design system.
> **Experience the simplicity of Bootstrap and the power of Tailwind together**

## Some Fetures
- An API for your design system.
- Build whatever you want, seriously.
- Responsive everything.
- Hover and focus states? We got em.
- Worried about duplication? Dont be.
- The possibility of different design in LTR and RTL direction

## Different Dark and light mode design
Dont want to be one of those websites that blinds people when they open it on their phone at 2am? Enable dark mode in your configuration file then throw dark: in front of any color utility to apply it when dark mode is active. Works for background colors, text colors, border colors, and even gradients.

## Websites designed with this design system
- Atiex Fiat & Crypto Exchange (https://atiex.uk)
- Hamtapay Crypto Currency Exchange (https://hamtapay.net)

## Css Comparison

A comparison of CSS library sizes

| Name                   | Version | Size (uncompressed) | Size (minified) | URL                                                   |
|------------------------|---------|---------------------|-----------------|-------------------------------------------------------|
| Hamtapay design system | v1.0.0  | 230 KB              | 130 KB          | https://github.com/devzarghami/scss-class-generator                               |
| Tailwindcss            | v1.0.0  | 2413.4 kB	         | 1967.4 kB	   | https://v1.tailwindcss.com/docs/controlling-file-size |
| Bootstrap              | v4.0.0  | 187 KB              | 147 KB          | https://v4-alpha.getbootstrap.com/                    |

## Online Scss to Css Compiler Website
- https://jsonformatter.org/scss-to-css
- https://www.cssportal.com/scss-to-css

## Usibility
Change the properties of each class according to your needs from **properties.scss**

**You can customize each class using the following features** *( dark:false, hover:false, responsive:false,direction:false, important:false )*
```css
@include utility($class: "v-bg", $source: "colors", $attribute: "background-color", $mode: (dark:true, hover:true));
```
Compiled output of the above code
```css
.v-bg-gray-50 {
  background-color: #F7F8FA;
}
.v-bg-gray-100 {
  background-color: #F2F3F5;
}
.v-bg-gray-200 {
  background-color: #E6E7EB;
}

.hover\:v-bg-gray-50:hover {
  background-color: #F7F8FA;
}
.hover\:v-bg-gray-100:hover {
  background-color: #F2F3F5;
}
.hover\:v-bg-gray-200:hover {
  background-color: #E6E7EB;
}

.dark .dark\:v-bg-gray-50 {
  background-color: #F7F8FA;
}
.dark .dark\:v-bg-gray-100 {
  background-color: #F2F3F5;
}
.dark .dark\:v-bg-gray-200 {
  background-color: #E6E7EB;
}

.dark .dark\:hover\:v-bg-gray-50:hover {
  background-color: #F7F8FA !important;
}
.dark .dark\:hover\:v-bg-gray-100:hover {
  background-color: #F2F3F5 !important;
}
.dark .dark\:hover\:v-bg-gray-200:hover {
  background-color: #E6E7EB !important;
}
```

## Examples

#### Dark & Light mode
Using Me to style your site in dark mode.
```html
<html>
	<body class="dark"> <!-- add 'dark' class to body to change to dark mode  -->

		<button class="v-bg-gray-500  dark:v-bg-gray-100">
			Save changes
		</button>
		
		<button class="v-bg-gray-500 hover:v-bg-gray-700 dark:v-gray-blue-100 dark:hover:v-gray-blue-100">
			Save changes
		</button>

	</body>
</html>
```

#### Rtl & Ltr Direction
```html
<html>
	<body class="rtl"> <!-- add 'rtl' class to body to change direction to RTL  -->

		<div class="v-width-100  v-text-left rtl:v-text-right">
			Lorem Ipsum
		</div>
		
		<button class="v-ml-3 rtl:v-mr-3">
			Lorem Ipsum
		</button>
		
		<button class="v-pl-3 rtl:v-pr-3">
			Lorem Ipsum
		</button>
		
	</body>
</html>
```

#### Responsive Design
Using responsive utility variants to build adaptive user interfaces.

`````css
 responsive:(
    sm:'min-width:640px',
    md:'min-width:768px',
    lg:'min-width:1024px',
    xl:'min-width:1280px',
    xxl:'min-width:1536px'
  ),
````
```html
<html>
	<body> <!-- when you change screen size  -->

		<p class="sm:v-font-size-10 md:v-font-size-12 lg:v-font-size-16 xl:v-font-size-18 xxl:v-font-size-22">
			Lorem Ipsum
		</p>

	</body>
</html>
```
#### Better spacer management
```css
spacer:(
    auto:auto,
    0: 0,
    1: 1 * .25rem,
    2: 2 * .25rem,
    3: 3 * .25rem,
    4: 4 * .25rem,
    5: 5 * .25rem,
    6: 6 * .25rem,
    7: 7 * .25rem,
    8: 8 * .25rem,
    9: 9 * .25rem,
    10: 10 * .25rem,
  ),
```
```html
<html>
	<body>

		<p class="v-mt-3  v-mb-8  v-ml-4  v-mr-9  v-pt-2  v-pb-1  v-pl-4  v-pr-7">
			Lorem Ipsum
		</p>
		
		<p class="v-mx-4  v-px-3">
			Lorem Ipsum
		</p>
		<p class="v-pr-4  v-pl-3  v-pt-5  v-pb-8">
			Lorem Ipsum
		</p>

	</body>
</html>
```

#### Grid System And Flex Basis
Quickly manage the layout, alignment, and sizing of grid columns, navigation, components, and more with a full suite of responsive flexbox utilities. For more complex implementations

**Grid Template Columns**
- v-grid-cols-1
- v-grid-cols-2
- v-grid-cols-3
- v-grid-cols-4
- v-grid-cols-5
- v-grid-cols-6
- v-grid-cols-7
- v-grid-cols-8
- v-grid-cols-9
- v-grid-cols-10
- v-grid-cols-11
- v-grid-cols-12
- v-grid-cols-none

**Grid Template Rows**
- v-grid-rows-1
- v-grid-rows-2
- v-grid-rows-3
- v-grid-rows-4
- v-grid-rows-5
- v-grid-rows-6
- v-grid-rows-none

**Grid Column Start / End**
- v-col-auto
- v-col-span-1
- v-col-span-2
- v-col-span-3
- v-col-span-4
- v-col-span-5
- v-col-span-6
- v-col-span-7
- v-col-span-8
- v-col-span-9
- v-col-span-10
- v-col-span-11
- v-col-span-12
- v-col-span-full
- v-col-start-1
- v-col-start-2
- v-col-start-3
- v-col-start-4
- v-col-start-5
- v-col-start-6
- v-col-start-7
- v-col-start-8
- v-col-start-9
- v-col-start-10
- v-col-start-11
- v-col-start-12
- v-col-start-13
- v-col-start-auto
- v-col-end-1
- v-col-end-2
- v-col-end-3
- v-col-end-4
- v-col-end-5
- v-col-end-6
- v-col-end-7
- v-col-end-8
- v-col-end-9
- v-col-end-10
- v-col-end-11
- v-col-end-12
- v-col-end-13
- v-col-end-auto

**Responsive variations also exist for .d-flex and .d-inline-flex.**
- v-d-flex
- v-d-inline-flex
- sm:v-d-flex
- sm:v-d-inline-flex
- md:v-d-flex
- md:v-d-inline-flex

**Responsive variations also exist for flex-direction.**
- v-flex-row
- v-flex-row-reverse
- v-flex-column
- v-flex-column-reverse

**Responsive variations also exist for justify-content.**
- v-justify-content-start
- v-justify-content-end
- v-justify-content-center
- v-justify-content-between
- v-justify-content-around

**Responsive variations also exist for align-items.**
- v-align-items-start
- v-align-items-end
- v-align-items-center
- v-align-items-baseline
- v-align-items-stretch

**Responsive variations also exist for align-self.**
- v-align-self-start
- v-align-self-end
- v-align-self-center
- v-align-self-baseline
- v-align-self-stretch

**Responsive variations also exist for flex-wrap.**
- v-flex-nowrap
- v-flex-wrap
- v-flex-wrap-reverse

**Responsive variations also exist for order.**
- v-order-0
- v-order-1
- v-order-2
- v-order-3
- v-order-4
- v-order-5
- v-order-6
- v-order-7
- v-order-8
- v-order-9
- v-order-10
- v-order-11
- v-order-12

**Responsive variations also exist for align-content.**
- v-align-content-start
- v-align-content-end
- v-align-content-center
- v-align-content-around
- v-align-content-stretch
