# Website - Development
> PIBG SAM10
***

[Go to website][1]

[1]:https://pibgsam10.netlify.app

***

## Getting started
Listed in `package.json > scripts` are run scripts. You can see available commands using `npm run`.

First, run `npm i` to install dependencies.

- `npm run clean` to clean output folder.  
- `npm run build` to generate production build.  
- `npm run watch` to run and watch for changes.  
- `npm start` is equivalent to `watch`.  
- `npm run build-watch` to clean, build then watch.  
- `npm run pre-deploy` to deploy on Netlify.  
- `npm run pro-deploy` to deploy and set to production.  

## Deployment

First create `./.netlify/state.json` containing `siteId`.
```json
{ "siteId": "<your site id>" }
```
Then run:
```sh
netlify deploy --prod --message "Deployment message" --open
```
See [netlify-cli commands](https://cli.netlify.com/commands/) for details.

***

Developed by [nikahmadz](https://nikahmadz.github.io/)
