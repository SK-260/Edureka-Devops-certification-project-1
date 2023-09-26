pipeline {
  agent none
  stages{
    stage ('Puppet Installation') {
      agent {
         label 'slave'
        }
      steps {
        sh '''wget https://apt.puppetlabs.com/puppet6-release-focal.deb
              sudo dpkg -i puppet6-release-focal.deb
              sudo apt-get update -y
              sudo apt-get install puppet-agent -y'''
        }
    }
  }
}