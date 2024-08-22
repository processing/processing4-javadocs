# Processing 4 Javadoc
This repository automatically generates the Javadoc for Processing 4 and hosts it on GitHub Pages at:

👉 https://processing.github.io/processing4-javadocs/

## Automated Javadocs Deployment

This repository uses a custom GitHub Actions workflow [`build-and-deploy-javadoc.yml`](https://github.com/processing/processing4-javadocs/blob/gh-pages/.github/workflows/build-and-deploy-javadoc.yml) to automatically generate and updates Javadocs in the `/docs` folder.

### How It Works

- **Scheduled Run:** The workflow is triggered every Monday at midnight (UTC) to ensure that the Javadocs are always up-to-date.
- **Manual Trigger:** You can also manually trigger the workflow if needed.
- **Javadocs Generation:** The workflow clones the `processing/processing4` repository, builds the Javadocs using `ant`, and copies the generated files to the `/docs` directory of this repository.
- **Update Source Files:** The updated Javadocs are committed and pushed to the `gh-pages` branch.
- **Deployment:** We've set "Deploy from branch" in the repo settings to trigger on push to the `gh-pages` branch.

This automation helps keep the Javadocs updated without requiring manual intervention.

## Legacy

The source files for the [Processing 3 Javadocs](https://processing.github.io/processing-javadocs/core/) can be found at https://github.com/processing/processing-javadocs

## License
The Processing 4 reference is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC-BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).
