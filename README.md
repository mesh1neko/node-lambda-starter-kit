# node-lambda-starter-kit

Enable to focus on cording with [node-lambda](https://github.com/motdotla/node-lambda).

[![CircleCI](https://circleci.com/gh/mesh1nek0x0/node-lambda-starter-kit.svg?style=shield)](https://circleci.com/gh/mesh1nek0x0/node-lambda-starter-kit)
<!-- add ci status badge -->

## :pushpin: Description
Suitable for minimal AWS Lambda.

## :white_check_mark: Features
<!-- list up your product features. -->
- WIP :sparkles: powered by node-lambda
- :art: support .editorconfig
- :shirt: support lint with [eslint](https://eslint.org/)
- :black_joker: support test&coverage with [jest](https://facebook.github.io/jest/)
- :arrows_counterclockwise: support [CircleCI](https://circleci.com/)

---

## :floppy_disk: Install
### Requirements
* node v8.10+
* yarn v1.3.2+

### Step
1. Install
```
$ git clone ...
$ yarn install
```

You can also fork this repository.

## :arrow_forward: Usage

*invoke local*
```
$ yarn invoke
```

*run test*
```
$ yarn test
```

*run eslint*
```
$ yarn lint
```

*deploy lambda*

※Setting up AWS-CLI configuration yet? see [here](https://docs.aws.amazon.com/cli/latest/userguide/cli-config-files.html)

At first, overwrite .env. Your lambda role arn & region & function name(OS X example bellow)
```
$ sed -i '' 's/\(AWS_ROLE_ARN=\).*/\1<your_lambda_arn>/' .env
$ sed -i '' 's/\(AWS_REGION=\).*/\1<your_region>/' .env
$ sed -i '' 's/\(AWS_FUNCTION_NAME=\).*/\1<your_lambda_name>/' .env
```

Then, you can deploy like bellow.
```
$ yarn deploy
```

## :information_source: Anything else
<!-- show how to test, how to contribute -->
Nothing

## :pencil: Author
[mesh1nek0x0](https://github.com/mesh1nek0x0)

## :clipboard: LICENCE
`node-lambda-starter-kit` is licensed under the [MIT](https://github.com/mesh1neko/node-lambda-starter-kit/blob/master/LICENSE) license.

`node-lambda-starter-kit` uses 3rd party libraries, each with their own license. These are found here.
