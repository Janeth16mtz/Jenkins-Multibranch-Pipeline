pipeline{
	agent any
		stages{
			STAGE 1{
				steps{
					script{
						env.VARIABLE="value"
					}
				}
			}
			
			STAGE 2{
				steps{
					script{
						echo ${VARIABLE}
					}
				}
			}
			STAGE ('Three'){
				steps{
					sh'echo "Step Three"'
				}
			}
		}
}
