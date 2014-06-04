#Multi language html content module for dnn  (BETA)
RSEHtmlModuleDNN is a DNN html module with content localization, based on Open Web Studio and DotNetNuke 7 - MIT licensed. (BETA) not for production use.


##Features


##Installation
For those who are familiar with OWS
* OWS:    from folder \OWS\... install configuration "RSEHtmlModule ows configuration.config" into ows.
* MSSQL:  from folder \SQL\...  create table, view and proc.
    prepare initial script: open "sql initialscript insert some default values.sql" with texteditor and  prepare these lines to your needs.

    declare @PortalID int = '22'    -your PortalID
    declare @externDB nvarchar(100) = 'mydnn.dbo.'	--name of secondary database. If you use DNN-DB, then value = 'dbo.'
    declare @externnameDB nvarchar(100) = 'mydnn'   --name of secondary database. If you use DNN-DB, then value = ''
    declare @MasterLanguage nvarchar(100) = 'de-DE'		--preferred locale for new items

    execute initial script
* install module "_RSE.RSEHtmlModule_01.00.00_Install.zip" to dnn
* install bootstrap 3.x to your skin
  <script src="<%= PortalSettings.HomeDirectory %>bootstrap/js/bootstrap.min.js" type="text/javascript"></script>
  <link rel="stylesheet" type="text/css" href="<%= PortalSettings.HomeDirectory %>bootstrap/css/bootstrap.min.css" />
* map "RSEHtmlModule.css" to your skin <link rel="stylesheet" type="text/css" href="/DesktopModules/RSE/RSEHtmlModule/RSEHtmlModule.css" />
* install ckeditor for dnn

take a look at example skin, how to use css and js.

##Dependencies
* DNN evoq content (formerly DotNetNUke) http://www.dnnsoftware.com/
* OpenWebStudio (ows) for DNN http://www.openwebstudio.com/
* Bootstrap 3.x http://getbootstrap.com/
* CKEditor https://dnnckeditor.codeplex.com/
* require jQuery, 1.7 or higher
* requires jquery-ui 1.8.16 or higher


##Upgrades and Pull Requests
We actively encourage you to upgrade this module and provide pull requests to share your awesome work! Please ensure that any changes you make are:
* Non-breaking changes
* Tested thoroughly against the latest version
* Documented with the JSDoc standard as the other methods are
* Update the changelog at the top of this file with your updates

###Thank you to everyone who takes their time to write updates to the module!


##Roadmap
* make it an installable package

##Example websites, build with 
* http://www.duritcast.de
* http://www.duritsteel.de

#License
This plugin and all code contained is Copyright 2014 MattOpen, Germany. You are granted a license to use this code / software as you wish, free of charge and free of restrictions under the MIT license. 

This project is updated and maintained by:
MattOpen http://www.mattopen.com