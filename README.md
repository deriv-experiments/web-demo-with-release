# Web Demo with Release

This project is to show how we can use GitHub with Actions to manager our SDLC.

## Stages

### Developing
- The developer creates a branch
- The developer creates a pull request
- A preview is deployed and a url commented on the pull request for every commit
- A tester (or QA) will test the preview link

### Merging
- Either the developer or QA will merge the PR
- Nothing get's deployed at this stage

### Releasing
- The release manager creates a release in GitHub (ticking the prerelease option)
- A preview is deployed and a url added to the release description
- A tester (or QA) will test the preview link
- The tester or release manager will remove the prerelase flag
- The site gets deployed to production

## Locally

To run the project locally:

```
git clone git@github.com:deriv-experiments/web-demo-with-release.git
cd web-demo-with-release
npm install
npm run build
```

Then server the `dist` directory with your favorite web server.
