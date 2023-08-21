# upload-artifact-as-is

Forked from https://github.com/kittaakos/upload-artifact-as-is. The credit goes there. 🏅

Inspired by [actions/upload-artifact](https://github.com/actions/upload-artifact). The credit goes there. 🏅

This GitHub Action uploads build artifacts, but unlike the original [actions/upload-artifact](https://github.com/actions/upload-artifact) GitHub Action, this one does not require the desired artifact `name`, but uses the original name of the files for the uploads. No artifact name customization is possible.

## Inputs

### `path`

**Required** A file, directory or wildcard pattern that describes what to upload.

## Example usage

```yaml
    - uses: sorenson-eng/upload-artifact-as-is@main
    with:
        path: path/to/artifactDir/ # or path/to/artifactDir or path/to/artifactFile or path/to/**/wildcard/*
```

Output:

![Screen Shot 2020-05-15 at 12 58 38](https://user-images.githubusercontent.com/1405703/82043527-0889a080-96ac-11ea-91ea-8025a1632fe3.jpg)
