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

    @include button($type: "primary", $icon: true, $size: "medium");
  

- $type (string) = `"primary"`, `"secondary-green"`, `"secondary-dark-grey"`, `"secondary-light-grey"`, `"tertiary-green"`, `"tertiary-grey"`, `"tertiary-white"`.
- $icon (boolean OR string) = `true`, `false` (default), `"icon-name"` `(e.g. 'person', 'gear', 'dollar-circle')`.
- $size (string) = null (default), "medium", "large"

Buttons default to having no icon, and the regular size and the type must be specified. 

The icon parameter can be set to true and the default icon `chevron-circle-inverse` will be used. Any other v2-icon can also be used by specifying its name e.g. `"person"`, `"gear"`, `"dollar-circle"`, etc.
