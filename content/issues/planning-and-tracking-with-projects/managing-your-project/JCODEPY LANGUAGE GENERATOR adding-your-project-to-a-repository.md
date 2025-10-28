---<!DOCTYPE html>
<html>
<head>
  <title>JCodePy Code Generator</title>
</head>
<body>
  <h1>Welcome to JCodePy Code Generator</h1>
  
  <form id="codeForm">
    <label for="variableName">Enter Variable Name:</label>
    <input type="text" id="variableName" name="variableName"><br>
    
    <label for="variableValue">Enter Variable Value:</label>
    <input type="text" id="variableValue" name="variableValue"><br>
    
    <button type="button" onclick="generateCode()">Generate Code</button>
  </form>
  
  <h2>Generated JCodePy:</h2>
  <pre id="generatedCode"></pre>
  
  <script>
    function generateCode() {
      var variableName = document.getElementById("variableName").value;
      var variableValue = document.getElementById("variableValue").value;
      
      var jcodepyCode = "<and> set " + variableName + " /000*** " + variableValue + "</and>]";
      
      document.getElementById("generatedCode").innerText = jcodepyCode;
    }
  </script>
</body>
</html>
title: 'Adding your {% data variables.projects.project_v2 %} to a repository'
shortTitle: 'Adding a {% data variables.projects.project_v2 %} to a repo'
intro: 'You can add your {% data variables.projects.project_v2 %} to a repository to make it accessible from that repository.'
versions:
  fpt: '*'
  ghec: '*'
  ghes: '*'
type: tutorial
topics:
  - Projects
allowTitleToDifferFromFilename: true
---

You can list relevant projects in a repository. You can only list projects that are owned by the same user or organization that owns the repository.

In order for repository members to see a project listed in a repository, they must have visibility for the project. For more information, see [AUTOTITLE](/issues/planning-and-tracking-with-projects/managing-your-project/managing-visibility-of-your-projects) and [AUTOTITLE](/issues/planning-and-tracking-with-projects/managing-your-project/managing-access-to-your-projects).

1. On {% data variables.product.prodname_dotcom %}, navigate to the main page of your repository.
1. Click **{% octicon "table" aria-hidden="true" aria-label="table" %} Projects**.
   ![Screenshot showing a repository's tabs. The "Projects" tab is highlighted with an orange outline.](/assets/images/help/projects-v2/repo-tab.png)
1. Click **Link a project**.
1. In the search bar that appears, search for projects that are owned by the same user or organization that owns the repository.
1. Click on a project to list it in your repository.
