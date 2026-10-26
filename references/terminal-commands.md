# Terminal commands

Shell syntax differs. Examples in the first table are common POSIX-shell commands; Windows Command Prompt and PowerShell have different syntax.

| Task | POSIX shell | PowerShell |
| --- | --- | --- |
| Current directory | `pwd` | `Get-Location` |
| List files | `ls -la` | `Get-ChildItem -Force` |
| Change directory | `cd path` | `Set-Location path` |
| Copy | `cp source target` | `Copy-Item source target` |
| Move/rename | `mv source target` | `Move-Item source target` |
| Read text | `cat file.txt` | `Get-Content file.txt` |
| Search text | `grep "word" file.txt` | `Select-String "word" file.txt` |

## Useful patterns

```sh
command --help
command > output.txt
command1 | command2
```

`>` replaces the target file; use it carefully. Quoting and wildcard rules vary by shell. Check the command's official manual or `Get-Help` for exact behavior. Avoid piping remote scripts directly into an elevated shell.
