<img src="https://raw.githubusercontent.com/heartexlabs/label-studio/master/images/ls_github_header.png"/>

![label-studio](https://img.shields.io/badge/Label%20Studio-V1.5.0-green) ![label-studio-frontend](https://img.shields.io/badge/Label%20Studio%20Frontend-V1.4.0-green) ![data-manager](https://img.shields.io/badge/Data%20manager-v2.0.5-green)

# Install locally

```
git clone https://github.com/trdat123/custom-label-studio.git
```

After clone git to local, you need to run **_yarn_** to install _concurrently_.

## Front-end:

### Install node modules for each project

You need to go to each frontend folder `label-studio-frontend`, `dm2` and `label-studio/label_studio/frontend` and install _node_modules_ by using **_yarn_**

Or you can run this command below to install all _node_modules_:

```
yarn install:all
```

## Back-end:

You can create new virtual environment by using **_pip_** if you want.
After that, following the step below:

```
cd label-studio-1.5.0
pip install -e .
python label_studio\manage.py makemigrations
python label_studio\manage.py migrate
```

# Build locally for development

Run following command below:

## Option 1: run front-end and back-end in two terminal:

To run all frontend webpack

```bash
yarn watch:dev
```

Open other terminal and run this command:

```
cd label-studio-1.5.0
python label_studio\manage.py runserver
```

## Option 2: run all front-end and back-end in one terminal:

```
yarn dev
```

# Build run product locally

```
yarn build:product
```

# Details

| Name | Folder name           |
| ---- | --------------------- |
| lsf  | Label_studio_frontend |
| dm2  | datamanager           |
| ls   | label-studio-1.5.0    |

# Description of command of scripts in package.json file:

| Command       | Description                                                            |
| ------------- | ---------------------------------------------------------------------- |
| install:lsf   | install _node_modules_ for folder **_lfs_**                            |
| install:dm2   | install _node_modules_ for folder **_dm2_**                            |
| install:ls    | install _node_modules_ for frontend folder in **_ls_**                 |
| install:all   | run three command above                                                |
| watch:lsf     | build webpack realtime when change code **_lsf_**                      |
| watch:dm2     | build webpack realtime when change code in folder **_dm2_**            |
| watch:ls      | build webpack realtime when change code in frontend folder in **_ls_** |
| watch:dev     | run three command below                                                |
| build:lsf     | build webback of **_lsf_**                                             |
| build:dm2     | build webpack of **_dm2_**                                             |
| build:ls      | build folder frontend folder in **_ls_**                               |
| start:server  | run server from root folder                                            |
| dev           | run both front-end and back-end in one terminal                        |
| build:fe      | build all front-end                                                    |
| build:product | build all front-end and run server                                     |
