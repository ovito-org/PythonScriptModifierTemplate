# PythonScriptModifierTemplate
Template for a custom Python script modifier that hooks into OVITO.

This repository contains a template for creating your own Python script modifier, which can be installed into OVITO using pip.

## Getting Started

1. Click the "Use this template" button to create a new repository.
2. Rename `src/ModifierName` to reflect the name of your modifier.
3. Implement your modifier in `src/ModifierName/__init__.py`. If your modifier needs access to more than one frame or frames from an external trajectory, you can uncomment and implement the `input_caching_hints` method. More details on this method can be found in the [OVITO documentation](https://www.ovito.org/docs/current/python/introduction/custom_modifiers.html#writing-custom-modifiers-advanced-interface). Otherwise, you can delete it.
4. Fill in the pyproject.toml file. Fields that need to be updated are enclosed in a descriptive `[[field]]` tag. Please make sure to set an OVITO version >=3.9 as a dependency. Depending on your needs, you can add additional fields to the pyproject.toml file. Information can be found [here](https://setuptools.pypa.io/en/latest/userguide/index.html).
5. Fill in the README_Template.md file the [[fields]] should guide you. Feel free to add other sections like "Images", "Citation", or "References" as needed.
6. Add meaningful examples to the Examples directory to help others understand the use of your modifier.
7. Pick a license for your project and replace the current (MIT) LICENSE file with your license. If you keep the MIT license please update the name and year in the current file.
8. Once you're done, rename README_Template.md to README.md, replacing this file.
