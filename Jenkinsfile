@Library('jenkinsfile-pipeline-library@issue_1') _

def buildArtifact = new BuildStage()
def deployQa = new DeployStage('qa')
def deployUat = new DeployStage('uat')
def deployProd = new DeployStage('prod')

buildArtifact.then(deployQa)
             .then(deployUat)
             .then(deployProd)
             .build()
