pipeline{
	agent any
		stages{
			stage ('First'){
				steps{
					sh 'echo "Listo!"'
				}
			}
			
			stage ('Second'){
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
