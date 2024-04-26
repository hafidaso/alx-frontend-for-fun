# sass_scss


### Task 0: Always Debugging!
**File:** [0-debug_log.scss](alx-frontend-for-fun/sass_scss/0-debug_log.scss)
```scss
@debug "Hello world";
```

### Task 1: Color variable
**File:** [1-color_variable.scss](alx-frontend-for-fun/sass_scss/1-color_variable.scss)
```scss
$main-color: #3D3D3D;

body {
  color: $main-color;
}

p {
  color: $main-color;
}
```

### Task 2: Colors
**File:** [2-color_variables.scss](alx-frontend-for-fun/sass_scss/2-color_variables.scss)
```scss
$main-text-color: #3D3D3D;
$main-bg-color: #6D6D6D;

body {
  color: $main-text-color;
  background-color: $main-bg-color;
}

p {
  color: $main-text-color;
}

h2 {
  background-color: $main-bg-color;
}
```

### Task 3: Nested tag
**File:** [3-nested_tag.scss](alx-frontend-for-fun/sass_scss/3-nested_tag.scss)
```scss
body {
  margin: 0;
  padding: 0;

  p {
    margin: 10px;
  }
}
```

### Task 4: Nested class
**File:** [4-nested_class.scss](alx-frontend-for-fun/sass_scss/4-nested_class.scss)
```scss
body {
  color: #3D3D3D;

  .red {
    color: #FF0000;
  }
}
```

### Task 5: Nested child
**File:** [5-nested_child.scss](alx-frontend-for-fun/sass_scss/5-nested_child.scss)
```scss
body {
  color: #3D3D3D;

  > .red {
    color: #FF0000;
  }
}
```

### Task 6: Nested hover
**File:** [6-nested_hover.scss](alx-frontend-for-fun/sass_scss/6-nested_hover.scss)
```scss
button {
  color: #FF0000;

  &:hover {
    color: #00FF00;
  }
}
```

### Task 7: Nested and nested again
**File:** [7-nested_deeper.scss](alx-frontend-for-fun/sass_scss/7-nested_deeper.scss)
```scss
body {
  font-size: 14px;

  h1 {
    font-size: 16px;

    &.smaller {
      font-size: 12px;
    }
  }
}
```

### Task 8: Margin mixin
**File:** [8-mixin_margins.scss](alx-frontend-for-fun/sass_scss/8-mixin_margins.scss)
```scss
@mixin set-margins($left, $right) {
  margin-left: $left;
  margin-right: $right;
}

body {
  @include set-margins(10px, 10px);
}

div {
  @include set-margins(15px, 15px);
}
```

### Task 9: Extended
**File:** [9-extend_list.scss](alx-frontend-for-fun/sass_scss/9-extend_list.scss)
```scss
.info {
  font-size: 12px;
}

.success {
  @extend .info;
  color: #00FF00;
}

.warning {
  @extend .info;
  color: #FF0000;
}
```

### Task 10: Import colors
**File:** [10-import_colors.scss](alx-frontend-for-fun/sass_scss/10-import_colors.scss)
```scss
@import '10-colors';

.red {
  color: $red;
}

.green {
  color: $green;
}

.blue {
  color: $blue;
}
```

### Task 11: For each
**File:** [11-loop_photos.scss](alx-frontend-for-fun/sass_scss/11-loop_photos.scss)
```scss
@import '11-photos';

@each $name in $list-names {
  .photo-#{$name} {
    background: image-url("photos/#{$name}.jpg") no-repeat;
  }
}
```

### Task 12: Loop Headers
**File:** [12-loop_header.scss](alx-frontend-for-fun/sass_scss/12-loop_header.scss)
```scss
@for $i from 1 through 5 {
  h#{$i} {
    font-size: #{$i}px;
  }
}
```

### Task 13: Columns and operators
**File:** [100-loop_col.scss](alx-frontend-for-fun/sass_scss/100-loop_col.scss)
```scss
@for $i from 1 through 4 {
  .col-#{$i} {
    width: (100% / $i);
  }
}
```

### Task 14: Media query #0
**File:** [101-media_query.scss](alx-frontend-for-fun/sass_scss/101-media_query.scss)
```scss
h1 {
  font-size: 20px;

  @media screen and (max-width: 320px)

 {
    font-size: 14px;
  }
}
```

### Task 15: Media query #1
**File:** [102-media_query.scss](alx-frontend-for-fun/sass_scss/102-media_query.scss)
```scss
h1 {
  font-size: 20px;

  @media screen and (max-width: 960px) {
    font-size: 18px;
  }

  @media screen and (max-width: 640px) {
    font-size: 16px;
  }

  @media screen and (max-width: 320px) {
    font-size: 14px;

    &.small {
      color: #1D1D1D;
    }
  }
}
```

### Task 16: Sort!
**File:** [103-sort_strings.scss](alx-frontend-for-fun/sass_scss/103-sort_strings.scss)
```scss
$list_to_sort: john anna zoe kim felicia carrie;

@debug $list_to_sort;
@debug "Sorted List: #{sort($list_to_sort)}";
```
