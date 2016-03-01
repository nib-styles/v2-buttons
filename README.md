# @nib-styles/v2-buttons

nib styled buttons.

## Installation

    npm install --save @nib-styles/v2-buttons

**Note:** Requires `Opens Sans` and `Roboto` fonts from Google Fonts:

```html
<link rel='stylesheet' href='//fonts.googleapis.com/css?family=Open+Sans:700|Roboto:700' />
```

## Usage

### Using mixins

```scss
@import "@nib-styles/v2-buttons";

.feature {
  &__cta {
    @include button('primary', $icon: 'person', $size: 'large')
  }
}
```

```html
<button class="feature__cta">
    Add a dependant
</button>
```

### Using compiled classes

```scss
@import "@nib-styles/v2-buttons/compiled";
```

```html
<button class="v2-button v2-button--primary v2-button--large v2-button--icon-on-right">
    Add a dependant <i class="v2-icon v2-icon--person v2-icon--smallest v2-icon--offset-descenders"></i>
</button>
```

See the pattern library or [example/example.html](example/example.html) a complete list of classes.

## Mixins

```scss
@include button($type, $icon: false, $size: null);
```

- `$type` Required. May be `primary`, `secondary-green`, `secondary-dark-grey`, `secondary-light-grey`, `tertiary-green`, `tertiary-grey` or `tertiary-white`.

- `$icon` Optional. If `false` no icon is displayed. If `true` the `chevron-circle-inverse` icon is displayed. May be the name of a `v2-icon` e.g. `person`, `gear`, `dollar-circle`.

- `$size` Optional. May be `medium` or `large`.
