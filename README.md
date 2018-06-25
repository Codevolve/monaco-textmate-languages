## monaco-textmate + grammars for most languages

See `grammars` for list all the languages this package ships with

This package exposes `LanguageRegistry` class which has sweet lookup functions for language grammars.

You can get Grammar/Tokenizer by either by language ID or file extension or even MIME type.

Not all grammars have been "registered/activated" for use due to lack of time, so PR's would be appreciated. To "register/activate" a language,
every directory in `grammars/` must have atleast one `[lang-ext].config.json` file that looks like this:

```json
{
    "id": "typescript",
    "scopeName": "source.ts",
    "extensions": [".ts"],
    "mimeType": ["application/typescript"]
}
```

## License

MIT
