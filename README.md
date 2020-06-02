# ansiso

*Ansiso* (aka *ansiso* aka *ANSISO*) is a keyboard layout mainly aimed at developers who are used to the Finnish ISO layout but want a layout that's better suited for development and have it similar enough everywhere – no matter the OS (Windows or macOS) or the physical keyboard layout (ANSI or ISO).

todo: picture of the layout

Ansiso's main features are:
1. Access `[`, `]`, `{` and `}` from the same ergonomic spot as in the US and UK layouts.
1. Access `<`, `>`, `/`, `|` and `\` consistently from the same keys no matter the OS or the physical layout (ANSI or ISO) you are switching between.
1. Access `ä`/`Ä` and `ö`/`Ö` from the same physical keys as the standard Finnish layout. `å` is moved under Alt(Gr) because there is no room for it.
1. All the keys are in the same* places on both ANSI and ISO physical layouts.

If you don't care about the last point, you should also consider the [Finner](https://github.com/ruohola/finner) layout if that suits you better.

\*) Except [`* '`] because of, you know, geometry. The actual key still behaves the same.

## Language support

Currently only Finnish layout variant is available but open a new issue to collaborate on other variants! Same goes for Linux versions of the layouts.

## Details

Ansiso basically has the opposite strategy compared to the [Swerty](http://johanegustafsson.net/projects/swerty/) layout.

It starts with the default Finnish keyboard layout and does a few opinionated but pragmatic changes to individual keys. These changes make room for the square and curly bracket characters to sit where they would sit on ANSI (on the `å` `Å` and `¨` `^` `~` buttons). Then the rest of the characters are shoved under shift and Alt(Gr) to keep them accessible. Finally, the positions of `<`, `>`, `/`, `|` and `\` are modified slightly to make them appear in the same place no matter what OS or the physical layout (ANSI or ISO) you are using.

Here's a list of the exact changes from the Finnish layout by each key. The standard PC naming is used but the Mac differences are highlighted on the individual character level:
- [`å Å`]:
  * normal press: `å` → `[`
  * shift + key: `Å` → `{`
  * Alt(Gr) + key: N/A → `å`
  * Alt(Gr) + shift + key: N/A → `Å`
- [`¨ ^ ~`]:
  * normal press: `¨` → `]`
  * shift + key: `^` → `}`
  * Alt(Gr) + key: `~` (not changed)
  * Alt(Gr) + shift + key: N/A → `^`
- [`§ ½`]:
  * normal press: `§` → `<`
  * shift + key: `½` (`°` on Macs) → `>`
  * Alt(Gr) + key: N/A → `§`
  * Alt(Gr) + shift + key: N/A → `½` (`°` on Macs)
- [`7 / {`]:
  * normal press: `7` (not changed)
  * shift + key: `/` (not changed)
  * Alt(Gr) + key: `{` (`todo` on Macs) → `|`
  * Alt(Gr) + shift + key: N/A (`todo` on Macs) → `\`

### Dead keys

The characters with [dead key](https://en.wikipedia.org/wiki/Dead_key) behavior in the original Finnish layout behave the same way in this layout. For instance, hitting Alt(Gr) + [`¨` `^` `~`] doesn't print `~` before you also hit the space bar. However, both `]` and `}` (accessible via the same key) appear instantly (like on US ANSI).

A "no dead keys" variant may come in the future.

### Limitations

* You lose access to `¨` compared to the original Finnish layouts.
* You will be able to enter some of the characters from multiple different keys (e.g. on Windows you can enter `\` both from the standard [`+`] key and from the new modified [`7`] key).
