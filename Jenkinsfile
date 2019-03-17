  node{
   stage('SCM Checkout'){
     git 'https://github.com/ali22oo/MYAPPCi'
   }
   stage('Email Notification'){
     mail bcc: '', body: 'Hi Welcome to jenkins email alerts Thanks', cc: 'alioo@hotmail.com', from: '', replyTo: '', subject: 'Testing CC', to: 'alioo@hotmail.com'

   }
   stage('Slack Notification'){
       slackSend baseUrl: 'https://hooks.slack.com/services/',
       channel: '#jenkins-pipeline-demo',
       color: 'good', 
       message: 'Welcome to Jenkins, Slack!', 
       teamDomain: 'javahomecloud',
       tokenCredentialId: 'slack-demo'
   }
}


