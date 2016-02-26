# buttons

nib styled buttons.

## Usage

    <button class="v2-button v2-button--primary v2-button--large v2-button--icon-on-right">
        Button with icon <i class="v2-icon v2-icon--person v2-icon--smallest v2-icon--offset-descenders"></i>
    </button>

See the pattern library or [example.html](example.html) for more examples.

**Note:** Uses `Opens Sans` and `Roboto` fonts from Google:

    <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Open+Sans:700|Roboto:700" />

## Building

    $ npm run build
    $ npm run example.build

**Note:** Requires SASS 3.3 to build


## Mixins

  @include button($type, $icon, $size);
  

$type (string) = primary, secondary-green, secondary-dark-grey, secondary-light-grey, tertiary-green, tertiary-grey, tertiary-white
$icon (boolean) = true, false (default)
$size (string) = null (default), medium, large

Initially the `chevron-circle-inverse` icon on the right of the button is the only option. Other icons and placements can still be added the old way by adding an `<i>` tag inside the button.