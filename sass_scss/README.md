                Sass & Scss
## General
What Sass means
How to write Sass & Scss file
What is the difference between Sass and Scss
What is the Sass preprocessing
How to declare a variable
How to use nested definition
How to import a Sass file
How to use mixins
How to declare extend/inheritance styles
How to manipulate operators

1. What does Sass mean?
Sass stands for Syntactically Awesome Stylesheets. It's a CSS preprocessor that extends CSS with features like variables, nested rules, mixins, and more to make writing styles easier and more organized.

2. How to write Sass & SCSS files?
    Sass: Uses indentation instead of curly braces and semicolons.
    Example:
    $primary-color: blue
    body
        background: $primary-color
    SCSS: Uses syntax similar to regular CSS (with curly braces and semicolons).
    Example:
        $primary-color: blue;
    body {
        background: $primary-color;
    }
You can write these in files with extensions:
    .sass for Sass
    .scss for SCSS

Here's a beginner-friendly explanation of Sass and SCSS concepts:

1. What does Sass mean?
Sass stands for Syntactically Awesome Stylesheets. It's a CSS preprocessor that extends CSS with features like variables, nested rules, mixins, and more to make writing styles easier and more organized.

2. How to write Sass & SCSS files?
Sass: Uses indentation instead of curly braces and semicolons.
Example:
sass
Copier le code
$primary-color: blue
body
  background: $primary-color
SCSS: Uses syntax similar to regular CSS (with curly braces and semicolons).
Example:
scss
Copier le code
$primary-color: blue;
body {
  background: $primary-color;
}
You can write these in files with extensions:

.sass for Sass
.scss for SCSS
3. What is the difference between Sass and SCSS?
    Sass: Uses a simpler syntax (no curly braces {} or semicolons ;).
    SCSS: Fully compatible with regular CSS, using braces and semicolons. Both work the same way, but SCSS is more common because it feels familiar to those who already know CSS.
4. What is Sass preprocessing?
    Sass preprocessing means converting Sass or SCSS code into regular CSS. Tools like sass or build systems (e.g., Webpack) handle this for you.
5. How to declare a variable in Sass?
    Use the $ symbol to define a variable.
    Example:
    $main-color: red;
    h1 {
      color: $main-color;
    }
6. How to use nested definitions?
    Nest styles to show their relationship and reduce duplication.
    Example:
    nav {
       ul {
        list-style: none;
        }
       li {
        display: inline-block;
          }
        }
    This compiles into:
    nav ul {
        list-style: none;
    }
    nav li {
        display: inline-block;
    }
7. How to import a Sass file?
    Use the @import rule to include other Sass/SCSS files.
    Example:
    @import 'buttons'; // Imports the _buttons.scss file
    Make sure the imported file starts with _ (e.g., _buttons.scss) to indicate it's a partial file.
8. How to use mixins?
    Mixins are reusable blocks of code. Use @mixin to define and @include to apply.
    Example:
    @mixin button-style {
        padding: 10px;
        border-radius: 5px;
    }

    button {
        @include button-style;
    }
9. How to declare extend/inheritance styles?
    Use @extend to share styles between selectors.
    Example:
    %base-style {
       font-family: Arial, sans-serif;
       color: black;
    }

    h1 {
        @extend %base-style;
    }
    p {
        @extend %base-style;
    }
10. How to manipulate operators?
    You can perform operations like addition, subtraction, etc., in Sass.
    Example:
    $base-padding: 10px;

    div {
        padding: $base-padding * 2; // 20px
    }
