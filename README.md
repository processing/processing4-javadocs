# Processing 4 Javadoc
This repository automatically generates the Javadoc for Processing 4 and hosts it on GitHub Pages at the following address:

👉 https://processing.github.io/processing4-javadocs/

### How It Works

This repository uses a custom GitHub Actions workflow [`build-and-deploy-javadoc.yml`](https://github.com/processing/processing4-javadocs/blob/gh-pages/.github/workflows/build-and-deploy-javadoc.yml) .

The workflow clones the `processing/processing4` repository, gets the commit corresponding to the latest release, builds the Javadocs using `ant`, and copies the generated files to the `/docs` directory of this repository. The updated Javadocs are then committed and pushed to the `gh-pages` branch.

We've set "Deploy from branch" in the repo settings to trigger on push to the `gh-pages` branch. Every time the `build-and-deploy-javadoc.yml` workflow completes, it will trigger a deploy to GitHub pages.

The workflow is triggered every Monday at midnight (UTC). A maintainer can manually trigger the workflow if needed.

## Legacy

The source files for the [Processing 3 Javadocs](https://processing.github.io/processing-javadocs/core/) can be found at https://github.com/processing/processing-javadocs

## License
The Processing 4 reference is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC-BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).
