# Processing 4 Javadoc
This repository automatically generates the Javadoc for Processing 4 and hosts it on GitHub Pages at:

👉 https://processing.github.io/processing4-javadocs/

## Automated Javadocs Deployment

This repository uses a custom GitHub Actions workflow [`build-and-deploy-javadoc.yml`](https://github.com/processing/processing4-javadocs/blob/gh-pages/.github/workflows/build-and-deploy-javadoc.yml) to automatically generate and updates Javadocs in the `/docs` folder.

### How It Works

The workflow clones the `processing/processing4` repository, builds the Javadocs using `ant`, and copies the generated files to the `/docs` directory of this repository. The updated Javadocs are then committed and pushed to the `gh-pages` branch.

The workflow is triggered every Monday at midnight (UTC) to ensure that the Javadocs are always up-to-date. You can also manually trigger the workflow if needed.

We've set "Deploy from branch" in the repo settings to trigger on push to the `gh-pages` branch. Every time the `build-and-deploy-javadoc.yml` workflow completes, it will trigger a deploy to GitHub pages.

This automation helps keep the Javadocs updated without requiring manual intervention.

## Limitations

Currently, the workflow sources the main branch of the `processing/processing4` repository to generate the Javadocs. As a result, the Javadocs reflect the latest changes in the main branch, which might include updates that haven't been included in an official release yet. This could lead to discrepancies between the documentation and the most recent stable release of Processing 4

## To Do
- [ ] Update the workflow to generate Javadocs based on the latest stable release instead of the `main` branch.

## Legacy

The source files for the [Processing 3 Javadocs](https://processing.github.io/processing-javadocs/core/) can be found at https://github.com/processing/processing-javadocs

## License
The Processing 4 reference is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC-BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).
