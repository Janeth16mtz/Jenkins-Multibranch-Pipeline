pipeline{
	agent any
		environment { 
        		EXCECUTE = 'False'
    		}
		stages{
			stage ('First'){
				environment{
					EXCECUTE = "True"
				}
			}
			
			stage ('Second'){
				 when {
					environment name: 'EXCECUTE', value: 'True'
				    }
				steps{
					sh 'echo "Updating Second Stage"'
				}
			}
			stage ('Third'){
				steps{
					sh 'echo "Step Three"'
				}
			}
		}
}
