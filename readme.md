# crowdin-push-bug-demo

## Reproduction

1. clone this repo
2. `cd <repo-path>`
3. `crowdin push`
4. Observe failure message on screen from crowdin CLI:

```
$ crowdin push
❌ Fetching project info
❌ Failed to collect project info. Please contact our support team for help
❌ Error from server: <Code: <empty_code>, Message: Cannot deserialize value of type `java.util.LinkedHashMap<java.lang.String,java.lang.Integer>` from Array value (token `JsonToken.START_ARRAY`)
 at [Source: (String)"{"firstLineContainsHeader":false,"importTranslations":false,"scheme":[]}"; line: 1, column: 70] (through reference chain: com.crowdin.client.sourcefiles.model.FileInfoResponseList["data"]->java.util.ArrayList[30]->com.crowdin.client.sourcefiles.model.FileResponseObject["data"]->com.crowdin.client.sourcefiles.model.File["importOptions"]->com.crowdin.client.sourcefiles.model.SpreadsheetFileImportOptions["scheme"])>

```
