Sass mixins
=========================================

About
-------------------------------------------------------------------

This is a collection of useful Sass mixins created during various personal projects.

Usage
-------------------------------------------------------------------

Clone the git repo in your SASS/SCSS project. Use @import to make it available in your files.

    git clone http://git@github.com:country/Sass-mixins.git
    
    // scss:
    @import 'Sass-mixins/mixins';

Mixins list
-------------------------------------------------------------------

### Arrow

Add an arrow on the side of the targeted element. Inspired by [CSSArrowPlease.com](http://cssarrowplease.com) by [Simon Højberg](https://twitter.com/shojberg)

#### Syntax:

    @include arrow([position], [size], [color], [borderWidth], [borderColor], [type]);

#### Arguments:

1. position - Position of the arrow, can be top, bottom, left or right. Defaults to top.
2. size - Size of the arrow. Defaults to 10px.
3. color - Color of the arrow. Defaults to black.
4. borderWidth - Width of the arrow's border. Defaults to 0 (no border).
5. borderColor - Color of the border. Defaults to transparent.
6. type - Type of the arrow, can be outside or inside. Defaults to outside.

#### Example:

    .my-box {
        border: 2px solid #C5C5C5;
        padding: 10px;
        @include arrow(left, 20px, #FFF, 2px, #C5C5C5);
    }

### Clearfix

Clear a float container.

#### Syntax:

    @include clearfix();

### Image replacement

Hide the textual content of the targeted element (Use the H5BP Image Replacement technique by [Nicolas Gallagher](http://nicolasgallagher.com))

#### Syntax:

    @include ir();