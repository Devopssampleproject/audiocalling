pipeline{
        agent {label 'master'}
        stages{ 
                stage('create branch'){
                        environment{
                        SECRET_FILE_ID = credentials('gitlogin_newbranch')}
        steps{
               // sh 'git checkout release/2021.11.01'
                sh 'git checkout -b test10-release/2021.11.01'
            //stdout = sh(script:'git checkout -b test-release/2021.11.01',  returnStdout: true)
            // println("GIT add stdout ################ " + stdout + " ####################")
            
            //withCredentials([usernamePassword(credentialsId: 'gitlogin_newbranch', passwordVariable: 'GIT_PASSWORD', usernameVariable: 'GIT_USERNAME')]) 
                //sh 'git config --global user.name "lakshmankumar2611"'
                //sh 'git config --global user.email "mlk.lucky836@gmail.com"'
                //sh 'git config --global  "mlk.lucky836@gmail.com"'
                sh 'git push https://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@github.com/Devopssampleproject/videocalling.git ' 
               // sh 'git push https://github.com/Devopssampleproject/videocalling.git test09-release/2021.11.01'
               // https://{TOKEN}@github.com/{USER}/{REPO}.git
                } //steps close
        
                } //stage close
        } //stages close
} //pipeline
