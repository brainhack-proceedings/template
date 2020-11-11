<h3 align="center"> Use this template </h3>
<h3 align="center"> 🍪✂️ </h3>

<p align="center">Click the green <code>Use this template</code> button and create a repository in your own user account. <br><br> Please follow <b>YYYY_MM_first-auth-surname_freeform-keywords</b> convention to name your repository. <br><br> For example: <code>2020_10_karakuzu_qmri-pulse-sequence</code></p>

<h3 align="center">  Create a GitHub access token </h3>
<h3 align="center"> 🔑 </h3>

<p align="center">Follow <a href="https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token#creating-a-token">these steps</a> and make sure that you check the <b>repo</b>, <b>admin:repo_hook</b> and <b>workflow</b> boxes while creating your access token.</p> 


<h3 align="center"> Create an encrypted secret for your repo </h3>
<h3 align="center"> 🕵️‍♀️ </h3>


<p align="center"> Simply follow <a href="https://docs.github.com/en/free-pro-team@latest/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository">these steps</a>.</p>

<p align="center">  The name of the secret must be <code>PAT_BHP</code> and the value must be the key you obtained from the previous step. </p>


<h3 align="center"> Push a dummy change to the <code>main</code> </h3>
<h3 align="center"> 📤 </h3>

<p align="center"> It can be anything, such as simply editing this <code>README.md</code> file you are reading at the moment. </p>

<h3 align="center"> What now ?  </h3>
<h3 align="center"> 👀 </h3>

<p align="center">After pushing your changes to the <code>main</code> branch, visit the <b>Actions</b> tab of your repository. You should see an action named <b>Report</b>, which consists of three jobs: <code>updateInfo</code> , <code>buildPDF</code> and <code>buildHugo</code>.</p>  

<p align="center">Soon after a successful action run, your web page will be deployed. You should see <b>Environments</b> section appeared in your repository (on the right column). In the <b>Environments</b> page, click the <code>View Deployment</code> button to visit your report page!

## Edit your report ✍️
  
* Place your figures in the [`figures`](figures) folder. 

* Edit [`report.md`](report.md) file to create your own report. The template markdown will walk you through how to cite references, add figures and equations etc.

* Edit [`report.bib`](report.bib) to add your bibliography in [BibTeX](http://www.bibtex.org/) format.

* To adjust the size and the appearence of your figures on the corresponging web-page, please edit <code>figures/figures.css</code> file. You can find the instructions in the file. 


| ⚠️ Warning|
| :--- |
|Please do not change the name or the location of [report.md](report.md) and [report.bib](report.bib).|

| Note|
| :--- |
|Your figures are expected to be located in the `figures` folder. This is strictly by design.|


**Whenever you push your changes to the `main` branch** (either directly or via merging a branch), GitHub [actions](/actions) will be triggered to update your report. That's it! 

If actions run completes successfully, 🟠 (running) will turn into ✅ (success). If your build fails, you will see ❌ instead. In that case, you can read the logs to see what went wrong.

**If you don't want to trigger a workflow run after pushing a commit to the `main` branch,** please pass `skip workflow` as the commit message.

## Wiki Page 

See a list of potential problems and their solutions at the [wiki page](https://github.com/brainhack-proceedings/template/wiki).
