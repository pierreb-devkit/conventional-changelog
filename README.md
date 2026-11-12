# :globe_with_meridians: WeAreOpenSource Conventional Changelog

## :book: Presentation

Prompts for [conventional changelog](https://github.com/conventional-changelog/conventional-changelog) standard, based on [cz-conventional-changelog](https://github.com/commitizen/cz-conventional-changelog), which seems to be abandoned. For this reason, we decided to make our own package and included some PRs, switch to ES6 and add an Emoji system for some fun.

Our rules on this dev, **Quick** / **Simple** / **Lite**.

![gif](https://github.com/weareopensource/conventional-changelog/blob/master/assets/demo.gif)

Quick links :

* [Global roadmap and  ideas about stacks](https://github.com/orgs/weareopensource/projects/3)

## :boom: Installation

Make sure you have installed all of the following prerequisites on your development machine:

- Node.js (10.x) - [Download & Install Node.js](https://nodejs.org/en/download/)

Local : 

```bash
npm install --save-dev @weareopensource/conventional-changelog commitizen
commitizen init @weareopensource/conventional-changelog --save-dev --save-exact
```

### Integration 

We suggest to follow something like this : [How to create good commit messages](https://medium.com/@klauskpm/how-to-create-good-commit-messages-67943d30cced). Juste change cz-conventional-changelog part with @weareopensource/conventional-changelog

### Configuration

#### package.json

Like commitizen, you specify the configuration of cz-conventional-changelog through the package.json's `config.commitizen` key.

```json5
{
// ...  default values
    "config": {
        "commitizen": {      
            "path": "./node_modules/cz-conventional-changelog",
            "maxHeaderWidth": 100,
            "maxLineWidth": 100,
            "defaultType": "",
            "defaultScope": "",        
            "defaultSubject": "",
            "defaultBody": "",
            "defaultIssues": ""
        }
    }
// ...    
}
``` 
### Environment variables

The following environment varibles can be used to override any default configuration or package.json based configuration.

* CZ_TYPE = defaultType 
* CZ_SCOPE = defaultScope
* CZ_SUBJECT = defaultSubject
* CZ_BODY = defaultBody
* CZ_MAX_HEADER_WIDTH = maxHeaderWidth
* CZ_MAX_LINE_WIDTH = maxLineWidth

### Commitlint

If using the [commitlint](https://github.com/conventional-changelog/commitlint) js library, the "maxHeaderWidth" configuration property will default to the configuration of the "header-max-length" rule instead of the hard coded value of 100.  This can be ovewritten by setting the 'maxHeaderWidth' configuration in package.json or the CZ_MAX_HEADER_WIDTH environment variable.


## :pencil2: Contribute

## :globe_with_meridians: [We Are Open Source, Who we are ?](https://pierreb.me)

Today, we dreams to create Backs/Fronts, aligns on feats, in multiple languages, in order to allow anyone to compose fullstack on demand (React, Angular, VusJS, Node, Nest, Swift, Go).
Feel free to discuss, share other kind of bricks, and invite whoever you want with this mindset to come help us.

Feel free to help us ! :)

## :clipboard: Licence

[MIT](/LICENSE.md)

## :link: Links

[Slack](https://join.slack.com/t/weareopensource/shared_invite/zt-62p1qxna-PEQn289qx6mmHobzKW8QFw) · [Discord](https://discord.gg/U2a2vVm) · [Mail](mailto:brisorgueilp@gmail.com?subject=Contact)
