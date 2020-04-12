# Render Comparison Tool

A tool for compariing UFG and Classic renders.

# Usage
- Options:
-  -v, --version                  output the current version
-  -k --key [key]                 Set your Applitools API Key. e.g. -k key (will default to APPLITOOLS_API_KEY in env)
-  -u --url [url]                 Add the site URL you want to generate a sitemap for. e.g. -u https://www.applitools.com (default:
                                 "https://www.random.org/integers/?num=100&min=1&max=100&col=5&base=10&format=html&rnd=new")
 - -sk --saucekey [saucekey]      Your Saucelabs key. Default: local headless chromedriver
 - -bn --batchname [batchname]    Name for the final comparison batch (default: "rct batch")
 - -vx --xdim [xdim]              X dimension of the viewport size. e.g. -vx 1600 (default: 1600)
 - -vy --ydim [ydim]              Y dimension of the viewport size. e.g. -vy 900 (default: 900)
 - -su  --serverurl [serverurl]   Set your Applitools  server URL. (Default: https://eyesapi.applitools.com). e.g. -v https://youreyesapi.applitools.com (default:
                                 "https://eyesapi.applitools.com")
 - -l --log [log]                 Enable Applitools Debug Logs (Default: false). e.g. --log (default: false)
 - -an --appname [appname]        Name of the application under test (default: "rct app")
 - -tn --testname [testname]      The name of the final comparison test in the Applitools batch (default: "rct test")
 - -sm --stitchmode [stitchmode]  The stitchmode to be used (Default: CSS) (default: "CSS")
 - -hl --headless [headless]      Run the browser headless (Default: false) (default: false)
 - -ml --matchlevel [matchlevel]  Run the browser headless (Default: false) (default: "Strict")
 - -b --browser [browser]         Use Chrome or FireFox (Default: Chrome) (default: "Chrome")
 - -en --envname [envname]        Set a custom prefix for the environment name assigned to the grid run (default: false)
 - -h, --help                     display help for command

## Installing

```sh
npm install [under construction]
```

## Using the package

```sh
rct-cli --h
```

## Troubleshooting

1) Baseline is the classic run instead of the visual grid
... The environment tag name was assigned to the classic run. It may not work to simply delete the tag or the environment record
... in the dashboard due to a bug. Instead, use the command line option 
