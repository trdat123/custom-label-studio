<img src="https://raw.githubusercontent.com/heartexlabs/label-studio/master/images/ls_github_header.png"/>


![label-studio](https://img.shields.io/badge/Label%20Studio-V1.5.0-green) ![label-studio-frontend](https://img.shields.io/badge/Label%20Studio%20Frontend-V1.4.0-green) ![data-manager](https://img.shields.io/badge/Data%20manager-v2.0.5-green)

# Install locally
```
git clone https://github.com/trdat123/custom-label-studio.git
```
After clone git to local, you need to run ***yarn*** to install *concurrently*.
### Frontend:
#### Install node modules for each project 

You need to go to each frontend folder `label-studio-frontend`, `dm2` and `label-studio/label_studio/frontend` and install node module by using ***yarn***

## Backend:
If you want you can create new virtual environment.
After that, following the step below: 
```
cd label-studio-1.5.0
pip install -e .
python label_studio\manage.py makemigrations
python label_studio\manage.py migrate
```
### Build locally for development
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
