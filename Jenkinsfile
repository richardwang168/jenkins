pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([parameters([
                        gitParameter(branch: '', branchFilter: 'origin/(.*)', 
                                defaultValue: 'main', 
                                description: 'Branch', 
                                name: 'Branch', 
                                quickFilterEnabled: false, 
                                selectedValue: 'TOP', 
                                sortMode: 'ASCENDING_SMART', 
                                tagFilter: '*', 
                                type: 'PT_BRANCH'
                            )
                        ])
                    ])
                }
            }
        }
        stage('Show branch-based-jenkinsFile') {
            steps {
                echo "This jenkinsfile is in devlop branch"
            }
        }
    }   
}
