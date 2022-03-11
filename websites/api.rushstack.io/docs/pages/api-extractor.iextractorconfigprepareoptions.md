---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@microsoft/api-extractor](./api-extractor.md) &gt; [IExtractorConfigPrepareOptions](./api-extractor.iextractorconfigprepareoptions.md)

## IExtractorConfigPrepareOptions interface

Options for [ExtractorConfig.prepare()](./api-extractor.extractorconfig.prepare.md) .

<b>Signature:</b>

```typescript
export interface IExtractorConfigPrepareOptions
```

## Properties

| Property                                                                                                | Type                                                                     | Description                                                                                                                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [configObject](./api-extractor.iextractorconfigprepareoptions.configobject.md)                          | [IConfigFile](./api-extractor.iconfigfile.md)                            | A configuration object as returned by [ExtractorConfig.loadFile()](./api-extractor.extractorconfig.loadfile.md) .                                                                                                                                                                                          |
| [configObjectFullPath](./api-extractor.iextractorconfigprepareoptions.configobjectfullpath.md)          | string \| undefined                                                      | The absolute path of the file that the <code>configObject</code> object was loaded from. This is used for error messages and when probing for <code>tsconfig.json</code>.                                                                                                                                  |
| [packageJson?](./api-extractor.iextractorconfigprepareoptions.packagejson.md)                           | [INodePackageJson](./node-core-library.inodepackagejson.md) \| undefined | <i>(Optional)</i> The parsed package.json file for the working package, or undefined if API Extractor was invoked without a package.json file.                                                                                                                                                             |
| [packageJsonFullPath](./api-extractor.iextractorconfigprepareoptions.packagejsonfullpath.md)            | string \| undefined                                                      | The absolute path of the file that the <code>packageJson</code> object was loaded from, or undefined if API Extractor was invoked without a package.json file.                                                                                                                                             |
| [projectFolderLookupToken?](./api-extractor.iextractorconfigprepareoptions.projectfolderlookuptoken.md) | string                                                                   | <i>(Optional)</i> The default value for the <code>projectFolder</code> setting is the <code>&lt;lookup&gt;</code> token, which uses a heuristic to guess an appropriate project folder. Use <code>projectFolderLookupValue</code> to manually specify the <code>&lt;lookup&gt;</code> token value instead. |
| [tsdocConfigFile?](./api-extractor.iextractorconfigprepareoptions.tsdocconfigfile.md)                   | TSDocConfigFile                                                          | <i>(Optional)</i> Allow customization of the tsdoc.json config file. If omitted, this file will be loaded from its default location. If the file does not exist, then the standard definitions will be used from <code>@microsoft/api-extractor/extends/tsdoc-base.json</code>.                            |