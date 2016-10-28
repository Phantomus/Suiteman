# Suiteman

Suiteman is a simple tool created to automate customization process of Suite Commerce Advanced applications.

Different types of files and resources in SuiteCommerce have different recommended best practices.
Newcomers are always confused how to choose the right one.
Moreover, even seasoned SCA veterans sometimes forget about company naming conventions and get annoyed when they need to do all copy/paste file manipulations.

Suiteman analyzes file path and creates all customization files in accordance with your company naming conventions.
Moreover, it automatically adds all required dependencies to appropriate place in distro.json file.

## Demo
<p align="center">
  <img src="https://github.com/Mykhail/Suiteman/raw/master/img/demo.gif" width="70%" alt="Suiteman's demo"/>
</p>

## Installation

To make Suiteman available to run across all of your SCA projects, we recommend installing it globally. You can do so using npm:

```
$ npm install suiteman -g
```


After that, you can run Suiteman on any SCA applications. Just run it in the root of Suite Commerce Advanced application :

```
$ suiteman PATH_TO_FILE

Example: suiteman Account@2.1.0/JavaScript/Account.Login.Model.js

```

## Configuration

Naming conventions from <a href="https://developers.suitecommerce.com/section4501068327">best practices for customizaing SCA</a> is used by default.

After running `suiteman --init`, you'll have a `.suiteman` file in the root directory of SCA.
Default settings could be changed here.

```json
{
    "customFolderName": "extensions",
    "customModuleFolderAfix": {
        "prefix": "",
        "suffix": ".Extension"
    },
    "customFileNameSuffix": ".Ext",
    "customModuleVersion": "1.0.0"
}
```

## Usage

To customize 
```
$ suiteman PATH_TO_FILE

Example: suiteman Account@2.1.0/JavaScript/Account.Login.Model.js

```
