<img src="https://raw.githubusercontent.com/heartexlabs/label-studio/master/images/ls_github_header.png"/>

![label-studio](https://img.shields.io/badge/Label%20Studio-V1.5.0-green) ![label-studio-frontend](https://img.shields.io/badge/Label%20Studio%20Frontend-V1.4.0-green) ![data-manager](https://img.shields.io/badge/Data%20manager-V2.0.0-green)

[Website](https://labelstud.io/) • [Docs](https://labelstud.io/guide/) • [Twitter](https://twitter.com/heartexlabs) • [Join Slack Community <img src="https://app.heartex.ai/docs/images/slack-mini.png" width="18px"/>](https://slack.labelstudio.heartex.com/?source=github-1)

## Install locally

```
git clone https://github.com/trdat123/custom-label-studio.git
```

## Install node modules for each project

You need to go to each frontend folder `label-studio-frontend`, `dm2` and `label-studio/label_studio/frontend` and install node module by using **_yarn_**

## Config .env file

you need to create .env file and paste into it. 
### Frontend folder in label studio 

```
NO_BUILD=true 
```

### Label-studio-frontend 

```
BUILD_NO_CHUNKS=true
BUILD_NO_HASH=true
BUILD_MODULE=true
NODE_ENV=production
```
### dm2

```
BUILD_NO_CHUNKS=true
BUILD_NO_HASH=true
BUILD_MODULE=true
NODE_ENV=production
```

## Build locally for development

Run following command below:

```bash
yarn build:dev
```

Open other terminal and run this command:

```
cd label-studio-1.5.0
python label_studio\manage.py runserver
```

## Build run product locally

```
yarn build:product
```

- Label Studio
- [Nginx](https://www.nginx.com/) - proxy web server used to load various static data, including uploaded audio, images, etc.
- [PostgreSQL](https://www.postgresql.org/) - production-ready database that replaces less performant SQLite3.

## Ecosystem

| Project                                                                               | Description                                                                                                                                                               |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| label-studio                                                                          | Server, distributed as a pip package                                                                                                                                      |
| [label-studio-frontend](https://github.com/heartexlabs/label-studio-frontend)         | React and JavaScript frontend and can run standalone in a web browser or be embedded into your application.                                                               |
| [data-manager](https://github.com/heartexlabs/dm2)                                    | React and JavaScript frontend for managing data. Includes the Label Studio Frontend. Relies on the label-studio server or a custom backend with the expected API methods. |
| [label-studio-converter](https://github.com/heartexlabs/label-studio-converter)       | Encode labels in the format of your favorite machine learning library                                                                                                     |
| [label-studio-transformers](https://github.com/heartexlabs/label-studio-transformers) | Transformers library connected and configured for use with Label Studio                                                                                                   |

## Roadmap

Want to use **The Coolest Feature X** but Label Studio doesn't support it? Check out [our public roadmap](roadmap.md)!

## Citation

```tex
@misc{Label Studio,
  title={{Label Studio}: Data labeling software},
  url={https://github.com/heartexlabs/label-studio},
  note={Open source software available from https://github.com/heartexlabs/label-studio},
  author={
    Maxim Tkachenko and
    Mikhail Malyuk and
    Andrey Holmanyuk and
    Nikolai Liubimov},
  year={2020-2022},
}
```

## License

This software is licensed under the [Apache 2.0 LICENSE](/LICENSE) © [Heartex](https://www.heartex.ai/). 2020-2021

<img src="https://github.com/heartexlabs/label-studio/blob/master/images/opossum_looking.png?raw=true" title="Hey everyone!" height="140" width="140" />
