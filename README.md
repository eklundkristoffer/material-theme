# Material Theme
Test

## Dependencies
+ Node/Yarn
+ Sublime Text 3
    + PackageDev

## Installation
```bash
git clone git@github.com:anomalyce/material-theme.git

ln -s material-theme ~/.config/sublime-text-3/Packages/Material\ Theme
```

## Compiling
```bash
yarn install
```

Make your changes to the files within the `./sources` directory.

**Notable Files**  
+ `./sources/settings/specific/Material-Theme-custom.json`
+ `./sources/themes/Material-Theme-custom.json`

**Notable Directories**  
+ `./sources/themes/custom/`
+ `./assets/accent-custom-magenta/`

### Theme
```bash
yarn run bt
```

### Scheme
```bash
yarn run bs
```

The above command will generate all of the YAML scheme files within the `./schemes` directory. Open your desired scheme file in Sublime Text.

```bash
subl3 ./schemes/Material-Theme-custom.yml
```

Launch the Command Palette (`Ctrl + Shift + P`) and search for `PackageDev: Convert (YAML, JSON, PList...)`. This should compile the opened `.yml` file into a `.tmTheme`.

```bash
mv ./schemes/Material-Theme-custom.tmTheme ./Material-Theme-custom.tmTheme
```

