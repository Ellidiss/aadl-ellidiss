# AADL support for Visual Studio Code

<table>
<tr>
<td>
    <p>
    This extension provides syntax highlight, error detection, multi file navigation and outlines for AADL files. It supports AADL 2.2 syntax.
    </p>
    <p>
    This extension is provided by <a href="https://www.ellidiss.com">Ellidiss Technologies</a>. For any question or problem,  contact us at <a href="mailto:support@ellidiss.com">support@ellidiss.com</a>.
    </p>
</td>
<td> <img src="https://www.ellidiss.fr/public/chrome/site/logoEllidiss.png" alt="Ellidiss logo"/> </td>
</tr>
</table>

![Syntax](assets/syntax.webp)

## Features

This extension contains a full AADL parser allowing error detection and reference resolution (go to definition or find references):

![Error](assets/errors.webp)

The reference resolution also allows for navigation between files:

![Navigation](assets/navigation.webp)

A full list of symbols is availaible using `Ctrl+P #` or `Cmd+P #`:

![Navigation](assets/symbols.webp)

A command named `AADL: Create Prolog statements from source` will create Prolog statements for the current AADL document. These statements are compatible with [AADLInspector](https://www.ellidiss.com/products/aadl-inspector/#1602496553568-50349c49-b4ce1b55-4004).

The command `AADL: Split file into one file for each package (OSATE compabitility)` split openned file into one file for each package.

## Extension Settings

This extension contributes the following settings:

* `aadl-ellidiss.maxDocumentSizeForParsing`: Maximum size for a document that can be parsed (in kilobytes). Default is 1024 kilobytes.

## Release Notes

### [0.8.0]

- Corrects parser error for range of with complex reference.
- Only load AIC file if present in a workspace.
- Reload units and AIC references upon configuration change.
- Better support for partial references resolution.
- Corrected error signalisation size.

### [0.7.0]

- Adds support for old AIC format.
- Reference resolution now support more cases (including multiple definitions).
- Adds support for partial reference resolution.
- Supports inverted feature groups.

### [0.6.0]

- Adds support for AADLInspector environment files.
- Now listens to workspace folders changes and external document openings.
- Few LAMP parsing fixes.

### [0.5.0]

- Adds command to run AADLInspector from an AADL or AIC file, with or without a plugin.
- Adds a tree view to present AIC projects in workspace

### [0.4.0]

- All AADL files present in the workspace are loaded upon activation of extension.
- Reference resolution is now incremental only updating current file and dependent units.
- Adds support for symbol rename.
- Shows all references for elements.

### [0.3.0]

- Corrects missing standard library preloading.
- Support for Behavior Annex syntax and reference checking.
- Better and more accurate reference resolution.

### [0.2.2]

- Corrects AADL commands on Windows failing with error `Command 'AADL: Create Prolog statements from source' resulted in an error`.

### [0.2.1]

- Supports corresponding embedded `{**` and `**}` tokens in annex
- Supports package splitting for OSATE compatibility with the Split command

### [0.2.0]

- Adds command to create Prolog statements from openned AADL document.
- Continue parsing with a missing semi-colon.
- Fix position for errors and navigation.

### [0.1.0]

Initial release of `aadl-ellidiss`
