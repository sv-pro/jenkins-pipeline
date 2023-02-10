
//checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sv-pro/jenkins-pipeline.git']])

node {
  stage('build') {
    echo 'Hi!'
    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sv-pro/jenkins-pipeline.git']])
    fruit = input (id: 'User_choice', message: 'pick one', ok: 'OK', parameters: [choice(choices: ['Apple', 'Banana', 'Peach'], description: 'Fruits', name: 'Fruit')])
    echo "$fruit"
  }
}
