# PrettyColors

![Carthage compatible](https://img.shields.io/badge/Carthage-✔-f2a77e.svg?style=flat)

## Description
`PrettyColors` is a Swift library for styling and coloring text in the Terminal.
The library outputs [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code) and conforms to [ECMA Standard 48](http://www.ecma-international.org/publications/standards/Ecma-048.htm).

### Example
```swift
import PrettyColors

let redText: String = Color.Wrap(foreground: .Red).wrap("A red piece of text.")
println(redText)

Color.Wrap(foreground: .Yellow, style: .Bold)
Color.Wrap(foreground: .Green, background: .Black, style: .Bold, .Underlined)

// 8-bit (256) color support
Color.Wrap(foreground: 114)
Color.Wrap(foreground: 114, style: .Bold)
```

**More examples can be found in [the tests](https://github.com/jdhealy/PrettyColors/blob/master/Tests/PrettyColorsTests.swift).**

### Installation
#### [Carthage](https://github.com/Carthage/Carthage#adding-frameworks-to-an-application)
Add the following to your Cartfile:

```ogdl
github "jdhealy/PrettyColors"
```

## Inspiration
- [`junegunn/ansi256`](https://github.com/junegunn/ansi256/)
- [`tehmaze/ansi`](https://github.com/tehmaze/ansi/)

## License
PrettyColors is released under the [MIT license](http://opensource.org/licenses/MIT). See [LICENSE.md](https://github.com/jdhealy/PrettyColors/blob/master/LICENSE.md) for details.
