pipeline{
	agent any
		stages{
			stage ('First'){
				steps{
					env.EXCECUTE = 'true'
					sh 'Listo!'
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
