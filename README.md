# action-script-diff

* Execute given script
* Generates a diff over a given file
* Verify if content of generated and commited files equals 

## Usage
``` yaml

- uses: nrfconnect/action-script-diff@v0.3
  with:
    # Path to file which should be inspected - relative to GitHub workspace
    diff_file: ''

    # Relative path and script name to be executed
    script_call: ''
```
