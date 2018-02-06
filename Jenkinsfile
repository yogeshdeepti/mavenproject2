node('node1') {
stage 'checkout'
checkout([$class: 'GitSCM', branches: [[name: '*/${BRANCH_NAME}']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5a02a237-d956-42c5-bdcc-866e9579480f', url: 'https://github.com/yogeshdeepti/mavenproject2.git']]])
stage 'build'
env.DIRPATH=pwd()
sh "echo ${env.DIRPATH}"
env.BRANCH=env.BRANCH_NAME
sh "echo ${env.BRANCH}"
sh "cd ${env.DIRPATH}/example" 
sh "mvn clean package"
}

