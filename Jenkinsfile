pipeline{
    agent any
        stages{
                stage ('1-clone'){
                    steps{
                        checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'groupgit', url: 'https://github.com/AppGroup2/jenkinsproject2.git']])

                        }   
                    }
                stage('2-Group Parallel job'){
                    parallel{
                        stage('Teeto-sub-job-1'){
                            steps{
                                sh 'lscpu'
                                sh 'echo $SHELL'
                            }
                        }
                        stage('Tolani'){
                            steps{
                            sh 'sudo systemctl status jenkins'
                            }
                        }
                    }
                }
                stage('3-Group Parallel job'){
                    parallel{
                        stage('Kayode'){
                            steps{
                                sh 'ls'
                            }
                        }
                        stage('Alade'){
                            steps{
                                sh 'pwd'
                            }
                        }
                    }
                }
                stage('4-Group Parallel job'){
                    parallel{
                        stage('Gabriel'){
                            steps{
                                sh 'lscpu'
                            }
                        }
                        stage('Tunde'){
                            steps{
                                sh 'pwd'
                            }
                        }
                        stage('Chris'){
                            steps{
                                sh 'whoami'
                            }
                        }
                    }
                }
    

            }   



    }
