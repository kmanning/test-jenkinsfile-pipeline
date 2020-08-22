@Library('jenkinsfile-pipeline-library') _

Jenkinsfile.init(this)

def buildArtifact = new BuildStage()
def deployQa = new DeployStage('qa')
def deployUat = new DeployStage('uat')
def deployProd = new DeployStage('prod')

buildArtifact.then(deployQa)
             .then(deployUat)
             .then(deployProd)
             .build()
