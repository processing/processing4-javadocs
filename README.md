# Processing 4 Javadoc
This repository automatically generates the Javadoc for Processing 4 and hosts it on GitHub Pages at the following address:

👉 https://processing.github.io/processing4-javadocs/

## How It Works

This repository uses a custom GitHub Actions workflow [`build-and-deploy-javadoc.yml`](https://github.com/processing/processing4-javadocs/blob/gh-pages/.github/workflows/build-and-deploy-javadoc.yml).

The workflow builds the Javadocs using `ant doc`, then copies the generated files to the `/doc` directory of this repository and deploys them to GitHub Pages.

## Legacy

The source files for the [Processing 3 Javadocs](https://processing.github.io/processing-javadocs/core/) can be found at https://github.com/processing/processing-javadocs

## License
The Processing 4 reference is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC-BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).
