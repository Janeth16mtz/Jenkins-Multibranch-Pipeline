pipeline{
	agent any
		stages{
			stage ('First'){
				steps{
					script{
						env.EXCECUTE="True"
					}
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
