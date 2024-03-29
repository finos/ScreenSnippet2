Badges go here (see [shields.io](https://shields.io/), for examples).

[![FINOS - Incubating](https://cdn.jsdelivr.net/gh/finos/contrib-toolbox@master/images/badge-incubating.svg)](https://finosfoundation.atlassian.net/wiki/display/FINOS/Incubating)

# ScreenSnippet2

Screen snippet tool for SDA.

## Dev requirements
OS: Windows
Visual Studio 2019 Enterprise edition
NodeJS v12  

## Execution

To execute the screen snippet tool, you'll need to open the Visual Studio Command prompt (Tools > Command prompt you added in Setup step) and run "npm run build".
This command will generate ```ScreenSnippet.exe``` file.

You can run this exe file in command line as follow:

```sh
> ScreenSnippet.exe --no-annotate
```

You will run screen snippet tool without annotation.
After capturing the screenshot, you will find a generated .png file.

## Debugging

Generate pdb file and execute the following in Visual Studio Command prompt:
```
>  cl ScreenSnippet.cpp /Zi
> devenv ScreenSnippet.exe
```
It will open Visual Studio. You just need to put your breakpoints and click on "Start". You will need to add "--no-annotate" argument.
## Contributing

1. Fork it (<https://github.com/symphonyoss/ScreenSnippet2/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Read our [contribution guidelines](.github/CONTRIBUTING.md) and [Community Code of Conduct](https://www.finos.org/code-of-conduct)
4. Commit your changes (`git commit -am 'Add some fooBar'`)
5. Push to the branch (`git push origin feature/fooBar`)
6. Create a new Pull Request

_NOTE:_ Commits and pull requests to FINOS repositories will only be accepted from those contributors with an active, executed Individual Contributor License Agreement (ICLA) with FINOS OR who are covered under an existing and active Corporate Contribution License Agreement (CCLA) executed with FINOS. Commits from individuals not covered under an ICLA or CCLA will be flagged and blocked by the FINOS Clabot tool. Please note that some CCLAs require individuals/employees to be explicitly named on the CCLA.

*Need an ICLA? Unsure if you are covered under an existing CCLA? Email [help@finos.org](mailto:help@finos.org)*


## License

Copyright 2019 Symphony LLC

Distributed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

SPDX-License-Identifier: [Apache-2.0](https://spdx.org/licenses/Apache-2.0)
