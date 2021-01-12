# Liam Extension / Plugin
A liam extension is a loadable extension that can be added into Liam at preparation, an extension comes with a custom event handler with multiple events that you can assign functions to.
The amount of functions you can add to a single event is unlimited but the recommended amount is 1-10 until stability assists are implemented.
You may only use Python files (no imports) and external markdown (no documentation) to store your extensions.

### `FileExtensions`
Documentation coming soon

### `Extensions`
No documentation yet

## How can I get my extension added to Liam?
Firstly, create a new folder with your extension file and a `contrib.json` file.
`contrib.json`:
```json
{"author": "example",
"contribution":
  {"name": "exampleextension",
  "filename": "extension.py",
  "events": ["on_bump", "on_setup", "on_bump_completed"]
  }
} 
```
Then zip the folder. After you have created the zipped folder, commit the file `Liam/plugins`.
