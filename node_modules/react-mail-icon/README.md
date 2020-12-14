<h1 align="center">
	<img alt="React Mail Icon" src="https://user-images.githubusercontent.com/16131737/65396536-0b6e0480-dd5c-11e9-896d-c11d0bc70e84.gif">
</h1>

> 📧 Simple, animated, and customizable mail icon.

## Install
```
$ npm install react-mail-icon
```

## Usage
```jsx
import React, { useState } from 'react'
import { MailIcon } from 'react-mail-icon'

const mailIconStyle = {
  display: 'flex'
} as React.CSSProperties

const App: React.FC = () => {
  const [shouldAnimate, setAnimation] = useState<boolean>(false)
  return (
    <div>
      <MailIcon
        style={mailIconStyle}
        mailBackFoldColor="#2874A6"
        mailTopFoldColor="#2E86C1"
        mailLeftFoldColor="#3498DB"
        mailRightFoldColor="#5DADE2"
        letterBackgroundColor="#FFFFFF"
        letterBorderColor="#1ABC9C"
        letterTextColor="#1ABC9C"
        shouldAnimateOpen={shouldAnimate}
        shouldAnimateDown={shouldAnimate}
        shouldAnimateOnHover
      />
      <button onClick={() => setAnimation(!shouldAnimate)}>Trigger animation</button>
    </div>
  )
}

export default App
```

## Props
#### style

Type: `Object`<br>
Optional: `true`

CSS styling for the component.

#### mailBackFoldColor

Type: `String`<br>
Default: `#2874A6`<br>
Optional: `true`

Color of the mail back fold.

#### mailTopFoldColor

Type: `String`<br>
Default: `#2E86C1`<br>
Optional: `true`

Color of the mail top fold.

#### mailLeftFoldColor

Type: `String`<br>
Default: `#3498DB`<br>
Optional: `true`

Color of the mail left fold.

#### mailRightFoldColor

Type: `String`<br>
Default: `#5DADE2`<br>
Optional: `true`

Color of the mail right fold.

#### letterBackgroundColor

Type: `String`<br>
Default: `#FFFFFF`<br>
Optional: `true`

Color of the letter background.

#### letterBorderColor

Type: `String`<br>
Default: `#1ABC9C`<br>
Optional: `true`

Color of the letter border.

#### letterTextColor

Type: `String`<br>
Default: `#1ABC9C`<br>
Optional: `true`

Color of the letter text.

#### shouldAnimateOpen

Type: `Boolean`<br>
Default: `false`<br>
Optional: `true`

If `true`, the mail should animate open and the letter should animate up.

#### shouldAnimateDown

Type: `Boolean`<br>
Default: `false`<br>
Optional: `true`

If `true`, the mail should animate down when opened.

#### shouldAnimateOnHover

Type: `Boolean`<br>
Default: `false`<br>
Optional: `true`

If `true`, the mail should animate when hovered (`shouldAnimateOpen` takes precendence).

## License
MIT
