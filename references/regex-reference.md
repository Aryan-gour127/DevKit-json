# Regular expression reference

Regex syntax depends on the engine. These common concepts are not identical in every language.

| Pattern | Meaning |
| --- | --- |
| `.` | Any character except line terminators in many modes |
| `\d` / `\w` / `\s` | Digit / word character / whitespace (engine-dependent) |
| `[abc]` | One character from a set |
| `[^abc]` | One character not in a set |
| `^` / `$` | Start / end of input or line, depending on mode |
| `*` / `+` / `?` | Zero-or-more / one-or-more / optional |
| `{m,n}` | Repetition range |
| `(abc)` | Capturing group |
| `(?:abc)` | Non-capturing group in engines that support it |
| `a|b` | Alternative |
| `\b` | Word boundary in many engines |

Escape metacharacters when you want them literally. Test against positive and negative examples, consider Unicode and multiline behavior, and avoid complex patterns that can cause excessive backtracking on untrusted input.

References: [MDN JavaScript regex guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions), [regex101](https://regex101.com/).
