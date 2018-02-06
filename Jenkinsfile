node('node1') {
stage 'checkout'
checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5a02a237-d956-42c5-bdcc-866e9579480f', url: 'https://github.com/yogeshdeepti/mavenproject2.git']]])
stage 'build'
sh "cd /var/lib/jenkins/workspace/multibranchtest1_master-RBLBEVWV6OIRNWDIRJTEIR6AI4DVUHT2EIQ2KFTVDIMUDVU7XGRQ/example" 
sh "mvn clean package"
}

