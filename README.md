# template-sandbox

[![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

This is a template for a Flutter project. 

This project was created to serve as a template for future Flutter projects. It includes internationalization, light and dark themes, and an app options class that can be used to store app-wide settings.



<!-- It includes a few things:
- Internationalization 
- Light and dark themes -->
<!-- - Basic responsiveness support -->

[flutter_starter_template.webm](https://user-images.githubusercontent.com/34327253/189505537-08e12361-eee5-4a2a-9d32-31f6c4fdd679.webm)


___

## Table of Contents
- [Background](#background)
- [Internationalization](#Internationalization)
- [Theme & app options](#Theme-&-app-options)
- [Contributing](#contributing)
- [Maintainers](#maintainers)
<!-- - [Responsiveness](#Responsiveness) -->


<!-- - [License](#license) -->


## Background

Internationalization is a feature that I find myself adding to most projects. But I find myself having to look up how to do every time I start a new project, so I wanted to have a template that I could use to quickly get started on a new project and support multiple languages, as well as multiple themes.

There are a few things that I would like to add in the future:
- Responsiveness support
- A more robust app options class

<!-- ## Usage -->
<!-- TODO: Fill out this section. -->

<!-- TODO: License -->
<!-- ## License -->

## Internationalization

This app is set up to support multiple languages.  

It is internationalized using the arb format. See [Internationalizing Flutter
apps
](https://docs.flutter.dev/development/accessibility-and-localization/internationalization#adding-your-own-localized-messages)
for more information.

To add a language, create a file in the `lib/l10n` directory and name it `intl_<language>.arb`. The file should contain a single arb file, with the following format:

```
{
    "appTitle": "Flutter Starter Template",
    "@appTitle": {
        "description": "The title of the app"
    }

    "appDescription": "This is a template for a Flutter project. It includes multiple language support, light and dark themes, andi is ready for responsive design.",
    "@appDescription": {
        "description": "App description"
    }

    ...
}
```
Use `AppLocalizations.of(context).nameOfTheKey` in the app to get the translation for the current locale.  

e.g. `AppLocalizations.of(context).appTitle` will return the translation for the key `appTitle` in the current locale.

Generated files are created when app is ran, and can be found under: `.dart_tool/flutter_gen/gen_l10n`


<!-- TODO: Add basic responsiveness support -->
<!-- ## Responsiveness

The app includes support for multiple screen sizes and orientations using the [responsive_builder](https://pub.dev/packages/responsive_builder) package. -->

<!-- The responsiveness logic is defined in `lib/layout/adaptive.dart`. -->

## Theme & app options
Themes are defined in `lib/core/app_themes_data.dart`.   
App options are defined in `lib/core/app_options.dart`.


## Contributing
PRs accepted.
<!-- Small note: If editing the README, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification. -->


## Maintainers  
**Lenz Paul**  
- gh: [@bringbackthedog](https://github.com/bringbackthedog/)    
- email: [lenz@gohash.tech](mailto:bringbackthedog@gmail.com)  
- linkedin: [linkedin.com/in/lenztpaul](https://www.linkedin.com/in/lenztpaul/)  
