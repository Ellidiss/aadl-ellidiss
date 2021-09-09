# Change Log

All notable changes to the "aadl-ellidiss" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

### [1.0]

- First public release
- Updated documentation

### [0.9]

- Adds a more robust reference resolution mecanism
- Presents duplication of element errors

### [0.8]

- Corrects parser error for range of with complex reference.
- Only load AIC file if present in a workspace.
- Reload units and AIC references upon configuration change.
- Better support for partial references resolution.
- Corrected error signalisation size.

### [0.7]

- Adds support for old AIC format.
- Reference resolution now support more cases (including multiple definitions).
- Adds support for partial reference resolution.
- Supports inverted feature groups.

### [0.6]

- Adds support for AADLInspector environment files.
- Now listens to workspace folders changes and external document openings.
- Few LAMP parsing fixes.

### [0.5]

- Adds command to run AADLInspector from an AADL or AIC file, with or without a plugin.
- Adds a tree view to present AIC projects in workspace

### [0.4]

- All AADL files present in the workspace are loaded upon activation of extension.
- Reference resolution is now incremental only updating current file and dependent units.
- Adds support for symbol rename.
- Shows all references for elements.

### [0.3]

- Corrects missing standard library preloading.
- Support for Behavior Annex syntax and reference checking.
- Better and more accurate reference resolution.

### [0.2.2]

- Corrects AADL commands on Windows failing with error `Command 'AADL: Create Prolog statements from source' resulted in an error`.

### [0.2.1]

- Supports corresponding embedded `{**` and `**}` tokens in annex
- Supports package splitting for OSATE compatibility with the Split command

### [0.2]

- Adds command to create Prolog statements from openned AADL document.
- Continue parsing with a missing semi-colon.
- Fix position for errors and navigation.

### [0.1]

Initial release of `aadl-ellidiss`
