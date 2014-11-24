# Gridlines

Gridlines is a Sass mixin that generates image-less grid backgrounds with ease. This eliminates having to create and recreate a bitmap image every time you want to experiment with a new set of measurements or viewport dimensions.

![940px](grid.png)

## Usage

1. Install with Bower (`bower install sass-gridlines`) or manually download [_gridlines.scss](_gridlines.scss) to your project’s directory.

2. Import the Sass partial.

3. Configure the mixin.

  ```scss
  body {
    @include gridlines(60px, 20px, 5px, 24px);
  }
  ```

4. Save countless hours!

### Arguments

The `gridlines` mixin takes four arguments. They are all optional—although, either `$width-column` or `$line-height` must be present—and in order, they are:

1. `$width-column`
2. `$width-gutter`
3. `$width-padding`
4. `$line-height`

### Variables

1. `$gl-vendor-prefix`: Sets the vendor prefix on linear-gradients. By default, this is "webkit".
