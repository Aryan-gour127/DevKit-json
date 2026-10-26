# Encoding and decoding tools

Encoding is not encryption. Base64, URL encoding, and hexadecimal do not protect secrets. Prefer local command-line tools for sensitive content.

## CyberChef

- **Website:** [gchq.github.io/CyberChef](https://gchq.github.io/CyberChef/)
- **Category:** Encoding and data transformation
- **Pricing:** Free and open source.
- **Best for:** Exploring chains of common encoding and transformation operations.
- **Key features:** Browser-based recipe workflow and many data operations.
- **Advantages:** Useful for learning and repeatable transformations.
- **Limitations:** Confirm whether processing stays in the browser for your use case; do not use it for confidential input without reviewing the implementation.
- **Official documentation:** [CyberChef repository](https://github.com/gchq/CyberChef)

## Base64 — MDN reference

- **Website:** [MDN Base64 glossary](https://developer.mozilla.org/en-US/docs/Glossary/Base64)
- **Category:** Encoding reference
- **Pricing:** Free.
- **Best for:** Understanding Base64 and browser APIs.
- **Key features:** Explanation and links to browser encoding/decoding APIs.
- **Advantages:** Maintained technical reference rather than an unknown converter.
- **Limitations:** Base64 provides no confidentiality.
- **Official documentation:** [MDN Web APIs](https://developer.mozilla.org/en-US/docs/Web/API)

## URL encoding — MDN reference

- **Website:** [MDN encodeURIComponent](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURIComponent)
- **Category:** URL encoding
- **Pricing:** Free.
- **Best for:** Correctly encoding a URI component in JavaScript.
- **Key features:** API behavior and examples.
- **Advantages:** Authoritative browser-language documentation.
- **Limitations:** URI components and full URLs have different encoding rules.
- **Official documentation:** [MDN URI encoding](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURI)

## Unicode reference

- **Website:** [Unicode Code Charts](https://www.unicode.org/charts/)
- **Category:** Character encoding reference
- **Pricing:** Free to access.
- **Best for:** Looking up Unicode code points and character blocks.
- **Key features:** Official code charts.
- **Advantages:** Primary source for the Unicode standard.
- **Limitations:** A character's appearance depends on fonts and rendering.
- **Official documentation:** [Unicode Standard](https://www.unicode.org/standard/standard.html)

## Base64.Guru

- **Website:** [base64.guru](https://base64.guru/)
- **Category:** Base64 encoding and decoding
- **Pricing:** Free to access; check current terms.
- **Best for:** Converting non-sensitive sample text or files.
- **Key features:** Browser-based Base64 conversion tools.
- **Advantages:** Focused interface for common conversions.
- **Limitations:** Base64 is not encryption; do not submit secrets or private files.
- **Official documentation:** [Base64.Guru tools](https://base64.guru/)
