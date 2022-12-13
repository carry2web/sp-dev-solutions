# Contribution Guidance

If you'd like to contribute to this repository, please read the following guidelines. Contributors are more than welcome to share your learnings with others from centralized location.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/)
or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Question or Problem?

Please do not open GitHub issues for general support questions as the GitHub list should be used for feature requests and bug reports. This way we can more easily track actual issues or bugs from the code and keep the general discussion separate from the actual code.  

## Typos, Issues, Bugs and contributions

Whenever you are submitting any changes to the SharePoint repositories, please follow these recommendations.

* Always fork repository to your own account for applying modifications
* Do not combine multiple changes to one pull request, please submit for example any samples and documentation updates using separate PRs
* If you are submitting multiple sample solutions, please create specific PR for each of them
* If you are submitting typo or documentation fix, you can combine modifications to single PR where suitable

## Submitting changes as pull requests

Here's a high level process for submitting new samples or updates to existing ones.

1. Sign the Contributor License Agreement (see below)
2. Fork the main repository to your GitHub account
3. Create a new branch for your fork for the contribution based on dev branch
4. Include your changes to your branch
5. Commit your changes using descriptive commit message - These are used to track changes on the repositories for monthly communications, see [May 2017](https://dev.office.com/blogs/PnP-May-2017-Release) as an example
6. Create a pull request in your own fork and target 'dev' branch
7. Fill up the provided PR template with the requested details

> note. Delete the feature specific branch only AFTER your pull request has been processed.

## Sample naming and structure guidelines

When you are submitting a new sample, it has to follow up below guidelines

- You will need to have a README file for your contribution, which is based on [provided template](../solutions/README-template.md) under the `solutions` folder. Please copy this template and update accordingly. README has to be named as README.md with capital letters.
    - You will need to have a picture of the web part in practice in the README file ("pics or it didn't happen"). Preview image must be located in /assets/ folder in the root your you solution.
- README template contains specific tracking image as a final entry in the page with img tag by default to https://pnptelemetry.azurewebsites.net/sp-dev-solutions/solutions/readme-template. This is transparent image, which is used to track popularity of individual samples in GitHub.
    - Updated the image src element according with repository name and folder information. If your sample is for example in samples folder and named as ChangeRequests, src element should be updated as https://pnptelemetry.azurewebsites.net/sp-dev-solutions/solutions/ChangeRequests
- If you find already similar kind of sample from the existing samples, we would appreciate you to rather extend existing one, than submitting a new similar sample
    - When you update existing samples, please update also README accordingly with information on provided changes and with your author details
- When you are submitting new sample solution, please name the sample solution folder accordingly
    - Name your folder based on the primary functionality of the component - for example, "ContactManagement"
    - Do not use words "sample", "solution", "extension", "webpart" or "wb" in the folder or sample name
- Do not use period/dot in the folder name of the provided sample

## Step-by-step on submitting a pull request to this repository

Please see following wiki post from the GitHub repository wiki for exact steps on submitting new pull requests. 

* How to submit a PR to SharePoint repository? - *Work in progress*

## Merging your existing github projects with this repository

If the sample you wish to contribute is stored in your own Github repository, you can use the following steps to merge it with the Psp-dev-solutions repository:

* Fork the sp-dev-solutions repository from GitHub
* Create a local git repository 

```
md sp-dev-solutions
cd sp-dev-solutions
git init
```

* Pull your forked copy of sp-dev-solutions into your local repository

```
git remote add origin https://github.com/yourgitaccount/sp-dev-solutions.git
git pull origin dev
```

* Pull your other project from github into the samples folder of your local copy of sp-dev-solutions

```  
git subtree add --prefix=samples/projectname https://github.com/yourgitaccount/projectname.git master
```

* Push the changes up to your forked repository

```
git push origin dev
```

Thank you for your contribution.  

> Sharing is caring. 