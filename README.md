<img align="left" src="Images/ReadMe/header2.png">

This Add-In is used to produce a timesheet file with functionality to import your Google Timeline. 

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/AnthonyDuguid/1.00)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE "MIT License Copyright © Anthony Duguid")
[![Latest Release](https://img.shields.io/github/release/Office-projects/Excel-Timesheet.svg?label=latest%20release)](https://github.com/Office-projects/Excel-Timesheet/releases)
[![Github commits (since latest release)](https://img.shields.io/github/commits-since/Office-projects/Excel-Timesheet/latest.svg)](https://github.com/Office-projects/Excel-Timesheet)

TODO: convert to .NET project and write up details of controls
* Tested on Windows 7 / Excel 2016

The most complete version is VBA. 
<a href="https://github.com/Office-projects/Excel-Timesheet/issues" target="_blank">
 <img alt="Issues" src="https://img.shields.io/github/issues/Office-projects/Excel-Timesheet.svg" />
</a>

<h1 align="left">
  <img src="Images/ReadMe/vba.excel.ribbon.timesheet.gif" />
</h1>

<br>

## Table of Contents
- <a href="#install">Install</a>
- <a href="#dependencies">Dependencies</a>
- <a href="#glossary-of-terms">Glossary of Terms</a>
- <a href="#functionality">Functionality</a> 
    - <a href="#ribbon-group-insert-data">Insert Data</a>
    - <a href="#ribbon-group-date-options">Date Options</a>
    - <a href="#ribbon-group-day-options">Day Options</a>
    - <a href="#ribbon-group-time-options">Time Options</a>
    - <a href="#ribbon-group-tools">Tools</a>
    - <a href="#ribbon-group-about">About</a>

<br>

<a id="user-content-install" class="anchor" href="#install" aria-hidden="true"> </a>
## Install
Instructions for installation of VBA version

### VBA
How to install the VBA version
1. Download the VBA Add-In file [![download VBA](https://img.shields.io/badge/download-VBA-brightgreen.svg)](https://github.com/Office-projects/Excel-Timesheet/raw/master/VBA/Timesheet.xlsm?raw=true "Download the VBA Add-In").

<br>

<a id="user-content-dependencies" class="anchor" href="#dependencies" aria-hidden="true"> </a>
## Dependencies
|Software                                   |Dependency                 |Project                    |
|:------------------------------------------|:--------------------------|:--------------------------|
|[Microsoft Visual Studio Community 2017](https://www.visualstudio.com/vs/whatsnew/)|Solution|VSTO|
|[Microsoft Office Developer Tools](https://visualstudio.microsoft.com/vs/features/office-tools/)|Solution|VSTO|
|[Microsoft Excel 2010 (or later)](https://www.microsoft.com/en-au/software-download/office)|Project|VBA, VSTO|
|[Visual Basic for Applications](https://msdn.microsoft.com/en-us/vba/vba-language-reference)|Code|VBA|
|[Extensible Markup Language (XML)](https://www.rondebruin.nl/win/s2/win001.htm)|Ribbon|VBA, VSTO|
|[Log4Net](https://www.nuget.org/packages/log4net/) |Error Logging |VSTO|
|[ScreenToGif](http://www.screentogif.com/)|Read Me|VBA, VSTO|
|[Snagit](http://discover.techsmith.com/snagit-non-brand-desktop/?gclid=CNzQiOTO09UCFVoFKgod9EIB3g)|Read Me|VBA, VSTO|
|Badges ([Library](https://shields.io/), [Custom](https://rozaxe.github.io/factory/), [Star/Fork](http://githubbadges.com))|Read Me|VBA, VSTO|

<br>

<a id="user-content-glossary-of-terms" class="anchor" href="#glossary-of-terms" aria-hidden="true"> </a>
## Glossary of Terms

| Term                      | Meaning                                                                                  |
|:--------------------------|:-----------------------------------------------------------------------------------------|
| COM |Component Object Model (COM) is a binary-interface standard for software components introduced by Microsoft in 1993. It is used to enable inter-process communication and dynamic object creation in a large range of programming languages. COM is the basis for several other Microsoft technologies and frameworks, including OLE, OLE Automation, ActiveX, COM+, DCOM, the Windows shell, DirectX, UMDF and Windows Runtime.  |
| VBA |Visual Basic for Applications (VBA) is an implementation of Microsoft's event-driven programming language Visual Basic 6 and uses the Visual Basic Runtime Library. However, VBA code normally can only run within a host application, rather than as a standalone program. VBA can, however, control one application from another using OLE Automation. VBA can use, but not create, ActiveX/COM DLLs, and later versions add support for class modules.|
| VSTO |Visual Studio Tools for Office (VSTO) is a set of development tools available in the form of a Visual Studio add-in (project templates) and a runtime that allows Microsoft Office 2003 and later versions of Office applications to host the .NET Framework Common Language Runtime (CLR) to expose their functionality via .NET.|
| XML|Extensible Markup Language (XML) is a markup language that defines a set of rules for encoding documents in a format that is both human-readable and machine-readable.The design goals of XML emphasize simplicity, generality, and usability across the Internet. It is a textual data format with strong support via Unicode for different human languages. Although the design of XML focuses on documents, the language is widely used for the representation of arbitrary data structures such as those used in web services.|
| KML|Keyhole Markup Language (KML) is an XML notation for expressing geographic annotation and visualization within Internet-based, two-dimensional maps and three-dimensional Earth browsers. KML was developed for use with Google Earth, which was originally named Keyhole Earth Viewer.|
<body>

<br>

<a id="user-content-functionality" class="anchor" href="#functionality" aria-hidden="true"> </a>
## Functionality
This Excel ribbon is inserted after the “Home” tab when Excel opens. Listed below is the detailed functionality of this application and its components.  



<a id="user-content-ribbon-group-insert-data" class="anchor" href="#ribbon-group-insert-data" aria-hidden="true"> </a>
### Insert Data (Group)
* Insert rows of data into the active table with the following controls.

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.insertdata.png" />
</h1>

####	Add Days (Button)
* Add days from the textbox values in the start and end dates in the "Date Options" group.

####	Add Timeline (Button)
* Add timeline events from downloaded .kml files from Google.

#### Download (Button)
* Download your Google timeline as .kml files. A file is created per day using the date filters in the ribbon.

#### Open Page (Button)
* Open your Google timeline web page.

#### UTC (Dropdown)
* This is the timezone offset for the stored date & time values in your Google Timeline.


<a id="user-content-ribbon-group-date-options" class="anchor" href="#ribbon-group-date-options" aria-hidden="true"> </a>
### Date Options (Group)
*...

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.dateoptions.png" />
</h1>

#### Start Date (Textbox)
*...

#### End Date (Textbox)
*...

#### Column (Combobox)
*...

#### Calendar (Button)
*...

#### Refresh (Button)
*...

#### Current Week (Button)
*...

#### Next 7 Days (Button)
*...

#### Filter Table (Button)
*...


<a id="user-content-ribbon-group-day-options" class="anchor" href="#ribbon-group-day-options" aria-hidden="true"> </a>
### Day Options (Group)
*...

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.dayoptions.png" />
</h1>

#### Sun, Mon, Tue, Wed, Thu, Fri, Sat (Checkboxes)
*...


<a id="user-content-ribbon-group-time-options" class="anchor" href="#ribbon-group-time-options" aria-hidden="true"> </a>
### Time Options (Group)
*...

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.timeoptions.png" />
</h1>

#### Start Date  (Combobox)
*...

#### End Date (Combobox)
*...

#### Break Time (Combobox)
*...

#### Refresh (Buttons)
*...

#### Start Date  (Textbox)
*...

#### End Date (Textbox)
*...

#### Break Time (Textbox)
*...


<a id="user-content-ribbon-group-tools" class="anchor" href="#ribbon-group-tools" aria-hidden="true"> </a>
###	Tools (Group)
*...

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.tools.png" />
</h1>


#### Settings (Button)
* Settings represent user preferences or valuable information the application needs to use.
   
<kbd>
VBA
<br>
  <img align="left" src="Images/ReadMe/vba.ribbon.settings.png" />
</kbd>

- VBA Settings
  - To add a new setting
    ```vbnet
    ThisWorkbook.CustomDocumentProperties.Add _
    Name:="App_ReleaseDate" _
    , LinkToContent:=False _
    , Type:=msoPropertyTypeDate _
    , Value:="31-Jul-2017 1:05pm"
    ```
  - To update a setting
    ```vbnet
    ThisWorkbook.CustomDocumentProperties.Item("App_ReleaseDate").Value = "31-Jul-2017 1:05pm"
    ```
  - To delete a setting
    ```vbnet
    ThisWorkbook.CustomDocumentProperties.Item("App_ReleaseDate").Delete
    ```

#### View Errors (Toggle Button)
*...

#### Export Code (Button)
*...


<a id="user-content-ribbon-group-about" class="anchor" href="#ribbon-group-about" aria-hidden="true"> </a>
###	About (Group)

<h1 align="left">
  <img src="Images/ReadMe/ribbon.group.about.png" />
</h1>


<a id="user-content-description" class="anchor" href="#description" aria-hidden="true"> </a>
#### Add-in Name (Label)
* The application name with the version

<a id="user-content-install-date" class="anchor" href="#install-date" aria-hidden="true"> </a>
#### Release Date (Label)
* The release date of the application

<a id="user-content-copyright" class="anchor" href="#copyright" aria-hidden="true"> </a>
#### Copyright (Label)
* The author’s name
