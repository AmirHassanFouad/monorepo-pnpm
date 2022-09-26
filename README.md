In package.json file: if you want your dependencies to always check within your
monorepo then you should prefix the version with "workspace:", example:
"@levelup/second": "workspace:1.0.0"

And if you want to not care about versioning at all then use "_" instead of the
version, example: "@levelup/second": "workspace:*"



in package.json root folder: "engines" property is used to determine which version should be installed/allowed to run this project


--Updating Packages and Version Syncing
use command: pnpm -r run update -i -L => -L: latest version