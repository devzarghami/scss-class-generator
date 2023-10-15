# VUI (Visual User Interface)

VUI, short for Visual User Interface, is a highly customizable and feature-rich utility class system built with SCSS. This framework is designed to simplify the process of creating well-engineered design systems and responsive web designs while keeping your stylesheets clean and consistent.

## Features

- **A Versatile API**: VUI provides an extensive API for your design system, offering a wide range of utility classes to help you maintain design consistency across your project.

- **Tailored Customization**: Build your designs according to your project's unique needs by customizing each class. Adjust colors, spacing, typography, and more effortlessly.

- **Seamless Responsiveness**: Create responsive designs with ease using utility classes that adapt to various screen sizes, ensuring a flawless experience on all devices.

- **Effortless Hover and Focus States**: Implement hover and focus states without writing additional CSS rules. VUI utility classes have you covered.

- **Support for Dark and Light Modes**: Enable dark and light mode designs effortlessly. Simply add the 'dark:' prefix to color utility classes for background colors, text colors, border colors, and gradients.

- **RTL (Right-to-Left) Ready**: Ensure your website is accessible to users who read from right to left. Use the 'rtl:' prefix to apply styles for RTL direction, making your design work seamlessly in diverse languages.

## Getting Started

To start using VUI in your project, follow these simple steps:

1. **Installation**: If you haven't already, include the VUI SCSS files in your project's SCSS workflow.

2. **Configuration**: Customize the classes according to your project's needs by editing the relevant SCSS files. You can control various features like dark mode, hover states, responsiveness, RTL support, and importance.

3. **Usage**: Start applying utility classes in your SCSS or HTML files. Use classes like 'v-bg-gray-500' for background colors, 'hover:v-bg-gray-700' for hover states, and 'dark:v-bg-gray-100' for dark mode styles.

## Documentation

For comprehensive information on how to use and customize VUI, refer to the official [documentation](link-to-your-documentation).

## Examples

Here are a few usage examples to give you a glimpse of how powerful and flexible VUI can be:

- **Dark & Light Mode**:

  ```scss
  .my-button {
    @include utility-class('v-bg-gray-500', (dark: 'v-bg-gray-100'));
  }
  ```

- **RTL & LTR Direction**:

  ```scss
  .my-content {
    @include utility-class('v-width-100', (direction: 'rtl:v-text-right'));
  }
  ```

- **Responsive Design**:

  ```scss
  .my-title {
    @include utility-class('v-font-size-16', (responsive: 'md:v-font-size-20 lg:v-font-size-24'));
  }
  ```

## Contribution

We warmly welcome contributions and feedback from the community. Feel free to contribute to the project, report issues, and help make VUI even more powerful. See our [contribution guidelines](link-to-contributing-guidelines) for more information.

## License

VUI is open-source and available under the [MIT License](link-to-license).

Embrace VUI and experience the simplicity and power it brings to your web development projects. Happy coding!
