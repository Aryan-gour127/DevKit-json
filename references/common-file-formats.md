# Common file formats

| Extension | Common use | Notes |
| --- | --- | --- |
| `.txt` | Plain text | Encoding matters; UTF-8 is common |
| `.md` | Markdown documentation | Rendered syntax varies by platform |
| `.json` | Structured data | Must follow JSON syntax; comments are not part of standard JSON |
| `.yaml` / `.yml` | Configuration and structured data | Indentation is significant |
| `.csv` | Tabular text data | Delimiters, quoting, and encoding vary |
| `.html` | Web document markup | A browser parses it with HTML rules |
| `.css` | Stylesheets | Used to describe presentation |
| `.js` / `.ts` | JavaScript / TypeScript source | TypeScript typically needs a build or runtime that supports it |
| `.xml` | Markup and structured data | Namespaces and schemas may apply |
| `.sql` | SQL statements | Dialect depends on the database |
| `.pdf` | Fixed-layout document | Not automatically searchable or accessible |
| `.png` | Lossless raster image | Supports transparency; often larger than compressed alternatives |
| `.jpg` / `.jpeg` | Compressed raster image | Lossy compression; no transparency |
| `.svg` | Vector image markup | Treat untrusted SVG as active content |
| `.zip` | Archive | Inspect contents before extracting untrusted files |
| `.gz` / `.tar` | Compressed file / archive | Common on Unix-like systems |

An extension is a hint, not proof of a file's contents or safety.
