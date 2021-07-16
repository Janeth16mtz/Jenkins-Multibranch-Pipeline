pipeline{
	agent any
		stages{
			stage ('One'){
				steps{
					script{
						env.VARIABLE="value"
					}
				}
			}
			
			stage ('Two'){
				steps{
					script{
						echo ${VARIABLE}
					}
				}
			}
			stage ('Three'){
				steps{
					sh 'echo "Step Three"'
				}
			}
		}
}
