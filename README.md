# PowerCLI Community Repository 
## Principles of Operations
[//]: # (LucD: Did you run this through Legal? Knowing the US habit of suing I want to make sure that every submitter's a** is covered.)
## Table of Contents
* [Abstract](https://github.com/vmware/PowerCLI-Example-Scripts#abstract)
* [Table of Contents](https://github.com/vmware/PowerCLI-Example-Scripts#table-of-contents)
* [Content Restrictions](https://github.com/vmware/PowerCLI-Example-Scripts#content-restrictions)
  * [Type of Content](https://github.com/vmware/PowerCLI-Example-Scripts#type-of-content)
* [Getting Started](https://github.com/vmware/PowerCLI-Example-Scripts#getting-started)
  * [Accessing the Repository](https://github.com/vmware/PowerCLI-Example-Scripts#accessing-the-repository)
  * [Adding Resources](https://github.com/vmware/PowerCLI-Example-Scripts#adding-resources)
* [Meta Information](https://github.com/vmware/PowerCLI-Example-Scripts#meta-information)
  * [Required Information](https://github.com/vmware/PowerCLI-Example-Scripts#required-information)
  * [Suggested Information](https://github.com/vmware/PowerCLI-Example-Scripts#suggested-information)
* [Suggested Quality Management](https://github.com/vmware/PowerCLI-Example-Scripts#suggested-quality-management)
  * [General Best Practices](https://github.com/vmware/PowerCLI-Example-Scripts#general-best-practices)
  * [Alias Usage](https://github.com/vmware/PowerCLI-Example-Scripts#alias-usage)
  * [Scripts](https://github.com/vmware/PowerCLI-Example-Scripts#scripts)
  * [Modules](https://github.com/vmware/PowerCLI-Example-Scripts#modules)
  * [Help Information](https://github.com/vmware/PowerCLI-Example-Scripts#help-information)
  * [Security](https://github.com/vmware/PowerCLI-Example-Scripts#security)
* [Resource Maintenance](https://github.com/vmware/PowerCLI-Example-Scripts#resource-maintenance)
  * [Maintenance Ownership](https://github.com/vmware/PowerCLI-Example-Scripts#maintenance-ownership)
  * [Filing issues](https://github.com/vmware/PowerCLI-Example-Scripts#filing-isssues)
  * [Resolving issues](https://github.com/vmware/PowerCLI-Example-Scripts#resolving-issues)
* [Additional Resources](https://github.com/vmware/PowerCLI-Example-Scripts#additional-resources)
  * [Discussions](https://github.com/vmware/PowerCLI-Example-Scripts#discussions)
  * [VMware Sample Exchange](https://github.com/vmware/PowerCLI-Example-Scripts#vmware-sample-exchange)
* [VMWARE TECHNOLOGY PREVIEW LICENSE AGREEMENT](https://github.com/vmware/PowerCLI-Example-Scripts#vmware-technology-preview-license-agreement)

## Abstract
This document will serve for collaboration to identify the operating principles of a centralized PowerCLI Community Repository on GitHub.   

The central PowerCLI repo will be located at: <https://github.com/vmware/PowerCLI-Example-Scripts>
## Content Restrictions
### Type of Content
The repository has been provided to allow the community to share resources that leverage VMware???s PowerCLI.  This can include:
* Sample Scripts
* Modules
* DSC Resources
* PowerActions scripts
* Pester Tests
* Tools built with PowerShell

## Getting Started
### Accessing the Repository
#### Downloading the Repository for Local Access
1. Load the GitHub repository page: <https://github.com/vmware/PowerCLI-Example-Scripts>
2. Click on the green ???Clone or Download??? button and then click ???Download ZIP???  
3. Once downloaded, extract the zip file to the location of your choosing  
4. At this point, you now have a local copy of the repository

#### Creating Your Own GitHub Based Access Point
1. Login (or signup) to GitHub
2. Load the GitHub repository page: <https://github.com/vmware/PowerCLI-Example-Scripts>
3. Click on the Fork button, which will create a copy of the repository and place it in the GitHub based location of your choosing. 

### Adding Resources
#### GitHub - Copy/Paste Option
1. Browse to the appropriate section (example: Scripts)
2. Select the ???Create new file??? button
3. On the new page, enter a file name, enter the resource???s information
4. Within the ???Commit new file??? area, enter the title and description, then select ???Create a new branch for this commit?????? and enter a sensical branch name
5. Click ???Propose new file???
6. On the ???Open a pull request??? page, click ???Create pull request???

#### GitHub - Upload files Option
1. Browse to the appropriate section (example: Modules)
2. Select the ???Upload files??? button
3. On the new page, drag or choose the files to add 
4. Within the ???Commit changes??? area, enter the title and description, then select ???Create a new branch for this commit?????? and enter a sensical branch name
5. Click ???Propose new file???
6. On the ???Open a pull request??? page, click ???Create pull request???

## Meta Information
This section will provide guidance on information which should be included with each submitted PowerCLI resource. Information listed in the Suggested Information will not be required for commit of a pull request to the repo, but will certainly increase ease of use for users of the resource.
### Required Information
The following information must be included with each submitted scripting resource. Please include the information in the appropriate location based upon the submitted scripting resource.  

* Author Name
  * This can include full name, Twitter profile, or other identifiable piece of information that would allow interested parties to contact author with questions.
[//]: # (LucD: Shouldn't we enforce that all question follow the Issues concept? Questions about a script might be useful for others.) 
* Date
  * Date the resource was written
* Minimal/High Level Description
  * What does the resource do
* Any KNOWN limitations or dependencies
  * vSphere version, required modules, etc.
[//]: # (LucD: Perhaps add a question to add additional "tested" versions/environments through the Issues concept. Original author(s) might not always have access.) 

#### Note Placement Examples:
Script:   Top few lines      
Module:   Module manifest  
  
#### Required Script Note Example:
`<#`  
`Script name:    script_name.ps1`  
`Created on:     07/07/2016`  
`Author:         Author Name, @TwitterHandle`  
`Description:    The purpose of the script is to ???`  
`Dependencies:   None known`  
`#>`  
[//]: # (LucD: Why not go for the standard PS Help format as a requirement?)
[//]: # (LucD: What about a Disclaimer? Or is that covered by the License attached to the repository?)
### Suggested Information
The following information should be included when possible. Inclusion of information provides valuable information to consumers of the resource.
* vSphere version against which the script was developed/tested
* PowerCLI build against which the script was developed/tested
* PowerShell version against which the script was developed/tested
* OS platform version against which the script was tested/developed
* Keywords that make it easier to find a script, for example: VDS, health check  

#### Suggested Script Note Example:
`<#`  
`Script name:    script_name.ps1`  
`Created on:     07/07/2016`  
`Author:         Author Name, @TwitterHandle`  
`Description:    The purpose of the script is to ???`  
`Dependencies:   None known`  

`===Tested Against Environment====`  
`vSphere Version: 6.0`  
`PowerCLI Version: PowerCLI 6.3 R1`  
`PowerShell Version: 5.0`  
`OS Version: Windows 10`  
`Keyword: VM`  
`#>`  

## Suggested Quality Management
This section describes guidelines put in place to maintain a standard of quality while also promoting broader contribution.
[//]: # (LucD: I'm missing the formatting of the code (capitalisation, indentation, aligned braces... Perhaps refer to the [The PowerShell Best Practices and Style Guide](https://github.com/PoshCode/PowerShellPracticeAndStyle))
### General Best Practices
### Resource Naming
* Give the resource a name that is indicative of the actions and/or results of its running

### Fault Handling
[//]: # (LucD: That article is a rather limited set of fault handling options. Shouldn't we add a snippet with some examples?)
* Read and apply the following basic fault handling where applicable: Microsoft???s Hey, Scripting Guy! Blog: https://blogs.technet.microsoft.com/heyscriptingguy/2014/07/09/handling-errors-the-powershell-way/

### Alias Usage
* Avoid any alias usage within all submitted resources.

### Global Variable Usage
* Avoid changing any global variables

### Help Information
* All resources should have inline documentation. 

### Scripts
* The script should be easy to read and understand
* Place user-defined variables towards the top of the script

### Modules
* The module file, PSM1, should contain only functions. A module manifest file, PSD1, should also be created and included. A module formatting file (format.ps1xml) is desirable but not a requirement.  
* Use only standard verbs

### Security
* Usage of PowerShell???s strict mode is preferred, but not required. 
* Remove any information related to one???s own environment (examples: Passwords, DNS/IP Addresses, custom user credentials, etc)

## Resource Maintenance
### Maintenance Ownership
Ownership of any and all submitted resources are maintained by the submitter. This ownership also includes maintenance of any and all submitted resources. 
[//]: # (LucD: This part is one of the reasons I asked about Legal and Disclaimers. Is Ownership the same as Liability?)
### Filing Issues
Any bugs or other issues should be filed within GitHub by way of the repository???s Issue Tracker. 
### Resolving Issues 
Any community member can resolve issues within the repository, however only the owner or a board member can approve the update. Once approved, assuming the resolution involves a pull request, only a board member will be able to merge and close the request. 

## Additional Resources
### Discussions
Join in on the discussion within the VMware Code Slack team's PowerCLI channel: <https://code.vmware.com/slack/>
[//]: # (LucD: I would suggest to start a dedicated Slack channel, for example "PowerCLI Repository". This to avoid having to look through all the PowerCLI clatter)
### VMware Sample Exchange
It is highly recommened to add any and all submitted resources to the VMware Sample Exchange: <https://developercenter.vmware.com/samples>
      
Sample Exchange can be allowed to access your GitHub resources, by way of a linking process, where they can be indexed and searched by the community. There are VMware social media accounts which will advertise resources posted to the site and there's no additional accounts needed, as the VMware Sample Exchange uses MyVMware credentials.     
[//]: # (LucD: Will that be an automated process?)

## VMWARE TECHNOLOGY PREVIEW LICENSE AGREEMENT
The VMware Technnology Preview License Agreement: <https://github.com/vmware/PowerCLI-Example-Scripts/blob/master/LICENSE.md>
[//]: # (LucD: This only protects VMware, not the submitters, as far as my legalese is correct)
# Repository Administrator Resources
## Table of Contents
* Board Members
* Approval of Additions

## Board Members

Board members are volunteers from the PowerCLI community and VMware staff members, board members are not held responsible for any issues which may occur from running of scripts inside this repository.
[//]: # (LucD: Again, I would like to have this checked by Legal. Especially for the submitter and the requirement to have a disclaimer in each script)

Members: 
* Josh Atwell (Community Member)
* Mathieu Buisson (Community Member)
* Luc Dekens (Community Member)
* Jonathan Medd (Community Member)
* Alan Renouf (VMware)
* Kyle Ruddy (VMware)
* Rynardt Spies (Community Member)

## Approval of Additions
Items added to the repository, including items from the Board members, require 2 votes from the board members before being added to the repository. The approving members will have ideally downloaded and tested the item. When two ???Approved for Merge??? comments are added from board members, the pull can then be committed to the repository.

[//]: # (LucD: What about Removals? Could imagine a submitter wants his submission removed)
 