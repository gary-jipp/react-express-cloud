

### Deploy Hook
- In Settings a Deploy hook is provided.
- lets try it
- Deployment triggered via deploy hook
- so now we know a deployment can be triggered from anywhere
- there is a whole WEB API for this
- https://api-docs.render.com/reference/create-deploy

### GitHub Actions
- using the Render API is really platform-specific.
- We'd like something more agnostic, not tied to the platform
- The MUCH more common way you'll see it is in GitHub Actions
- Go to the GitHub and select "Actions":  Empty
- lots of common "workFlow" examples.  OpenShift, Azure, Amazon (AWS)
- Obviously a lot of 'Azure' since Microsoft owns GitHub :)
- Render is not on the list.  But it exits. Google Search
- https://github.com/marketplace/actions/render-deploy-action
- Render Deploy Action

### Creating a GitHub Action
- we will disable auto-reploy in render: AutoDeploy = No in
- Now changes to the repo will not triger a build
- `.github/workflows` directory
- deployment files are written in YAML
- YAML is actually a superset of json
- we could write actions in JSON, but no one does that!
- call the workflow file `render.yaml`
- we could have actiond to deploy to other systems also
- we'll just copy and paste the example provided
- Change the name, add a manual deploy:  `workflow_dispatch:`
- push changes and you'll see your Action.
- Actions are always on the "default" branch (master or main)
