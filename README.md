# combine-svgs

---

Merge multiple svgs into one using `<symbol>` elements and optimizing with
[svgo](https://github.com/svg/svgo). Similar to
[grunt-svgstore](https://github.com/FWeinb/grunt-svgstore) and
[gulp-svgstore](https://github.com/w0rm/gulp-svgstore) and based on [Chris
Coyier's CSS Tricks
Article](https://css-tricks.com/svg-symbol-good-choice-icons/). Unlike the
previous two tools, I wanted something you could use regardless of what tools
you use.

## Usage

Currently, the program takes two arguments. The source directory containing the
svgs to be merged, and a target directory to place the result. For example:

    ./combine-svgs ./src/icons ./icons

Currently, the program will add `id` attributes to each `<symbol>` element based
on the name of the input file. So _my-icon.svg_ will have id _#my-icon_.

## Contributing

I built this because the other options I saw would require me to use Gulp or
Grunt, which I was unwilling to do. I hope this helps others that are in a
similar position.

I realize it is a very basic tool right now. If you wish to contribute or modify
it to suit your needs, feel free to submit a pull request so everyone can
benefit from your efforts! Also, please try to follow PEP8 style.
