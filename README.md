# Trailhead - Event Proposal Builder

A proposal-builder app for event planning, with an AI polish-draft feature, drafts saved locally in your browser, and a one-click text export.

## Hosting

GitHub Pages serves the built app. Settings -> Pages -> Source -> GitHub Actions. Every push to main runs the workflow in .github/workflows, which builds, runs the tests, and deploys only if the tests pass.

## Making changes

1. Ask Claude to edit src/App.jsx. Claude runs the test suite before handing it back.
2. 2. Update src/App.jsx in this repo.
   3. 3. GitHub Actions rebuilds, retests, and redeploys automatically.
     
      4. ## Polish draft feature
     
      5. Calls Claude from each person's browser, so each person enters their own Anthropic API key (API key button in the app). The key stays in that browser's local storage and is never committed here. If your network blocks api.anthropic.com, Polish will not work; everything else does.
     
      6. ## Local development
     
      7. npm install, then npm run build, then npm test.
      8. 
