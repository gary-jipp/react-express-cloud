
### Deploy to Clound
- many services.  We'll use Render
- free account
- deploy "New Web Service" (different for each)
- Build and Deploy from GitHub
- Connect our GitHub Repo.  Give permission
- Can give selective permission. by repository
- Set "Application" permission in GitHub Settings
- Select one or more repos that render can "see"
- "Connect" it to Render
- select `master` branch for now
- "Build Command" & "Start Command"
- Select Free :   0.1 CPU !! (not much but all we need)
- Any env settings:  remember .env?
- can also set the node version to be safe.  Match our own
- Takes about 2-3 minutes to deploy. (its 0.1 CPU!)
- Look at "Events" and wait
- Sure glad we're not using CRA for React now!
