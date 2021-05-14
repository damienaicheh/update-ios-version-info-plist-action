# Update iOS version Info.plist action

This action update the `BundleShortVersionString` and `BundleVersion` properties of the Info.plist file for your iOS projects.

## Inputs

### `info-plist-path`

**Required** The relative path for the Info.plist file.

### `bundle-short-version-string` 
  
**Required** The CF Bundle Short Version String.

###  `bundle-version`
    
**Required** The CF Bundle Version.

###  `print-file`

Output the Info.plist file in console before and after update.

## Usage

```yaml
- name: Update Info.plist
  uses: damienaicheh/update-ios-version-info-plist-action@1.0.0
  with:
    info-plist-path: './path_to_your/Info.plist'
    bundle-short-version-string: '2.0'
    bundle-version: '2'
    print-file: true
```