1. https://www.bacancytechnology.com/blog/deploy-angular-12-application-using-firebase-hosting/amp
2. https://talent500.co/blog/how-to-deploy-angular-12-application-using-firebase-hosting/
3. https://firebase.google.com/codelabs/firebase-web-io23#4
4. https://fireship.io/lessons/deploy-multiple-sites-to-firebase-hosting/
5. https://medium.com/@bpraveen.in/how-to-manage-dev-and-prod-projects-in-firebase-with-angular-and-firebase-hosting-10c335bb9437
6. https://medium.com/@luazhizhan/how-to-deploy-multiple-sites-to-firebase-hosting-part-1-a56949876c64
7. https://fireship.io/lessons/deploy-multiple-sites-to-firebase-hosting/
# host multi site projects
## step 1
```
{
  "hosting": [
    {
      "target": "admin",
      "public": "dist/admin-frontend",
      "ignore": [
        "firebase.json",
        "**/.*",
        "**/node_modules/**"
      ],
      "rewrites": [
        {
          "source": "**",
          "destination": "/index.html"
        }
      ]
    },
    {
      "target": "main",
      "public": "dist/main-frontend",
      "ignore": [
        "firebase.json",
        "**/.*",
        "**/node_modules/**"
      ],
      "rewrites": [
        {
          "source": "**",
          "destination": "/index.html"
        }
      ]
    }
  ]
}

```
## step 2

```
firebase target:apply hosting (targetname) (sitename)
firebase deploy --only hosting


```
