# this is a markdown

| column 1 | column 2|
| ---- | ---- |
| test 1 - fenced pipe | `dotnet test --filter "FullyQualifiedName~TestClass1|Category=Nightly"`|
| test 2 - non-fenced, escaped pipe | dotnet test --filter "FullyQualifiedName~TestClass1\|Category=Nightly" |
| test 3 - non-fenced, HTML coded pipe | dotnet test --filter "FullyQualifiedName~TestClass1&#124;Category=Nightly" |
| test 4 - "fenced" with HTML `<code>` tag (the **workaround**) | <code>dotnet test --filter "FullyQualifiedName~TestClass1&#124;Category=Nightly"</code> |
