# Play Catalog Contracts

Common Catalog Contract DTOs

## Create and Publish package
```s
VERSION=1.3.0
OWNER="playhuborg"
GH_PAT=[GitHubToken]

dotnet pack --configuration Release -p:PackageVersion=$VERSION -p:RepositoryUrl=https://github.com/$OWNER/lib-play-catalog-contracts -o ../packages

dotnet nuget push ../packages/Play.Catalog.Contracts.$VERSION.nupkg --api-key $GH_PAT --source "github"
```
