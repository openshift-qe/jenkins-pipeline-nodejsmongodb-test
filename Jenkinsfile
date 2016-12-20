node('nodejs') {
stage 'build'
openshiftBuild(buildConfig: 'nodejs-mongodb-example', showBuildLogs: 'true')
stage 'deploy'
openshiftDeploy(deploymentConfig: 'nodejs-mongodb-example')
stage 'check npm version'
sh 'npm --version'
}
