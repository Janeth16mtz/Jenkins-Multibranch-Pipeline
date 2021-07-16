pipeline{
	agent any
		stages{
			stage ('First'){
				environment{
					EXCECUTE = 'True'
				}
				steps{
					sh 'echo "Listo!"'
				}
			}
			stage ('Second'){
				when{
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
