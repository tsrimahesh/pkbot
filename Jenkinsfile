    node {

      stage ('Prepare environment') {

	    git branch: 'master', url: 'https://github.com/shreddy-pk/pkbot.git '
  

	          }

      stage ('Prepare environment') {

		        sh 'ssh -p2244 pkbot@118.102.131.235 sudo yum install epel-release'
			      sh 'ssh -p2244 pkbot@118.102.131.235 sudo yum install nodejs npm'
			          }

      stage ('Deploy') {

		          sh 'ssh -p2244 pkbot@118.102.131.235 git clone https://github.com/shreddy-pk/pkbot.git'
					  	sh 'ssh -p2244 pkbot@118.102.131.235 "cd pkbot && npm install hubot-slack --save"'
							sh 'ssh -p2244 pkbot@118.102.131.235 export HUBOT_ADAPTER=slack'
					    sh 'ssh -p2244 pkbot@118.102.131.235 export HUBOT_SLACK_TOKEN=xoxb-316277351014-4hTDsK3Om2TUOxRhuOa8Jnrd'
			        sh 'ssh -p2244 pkbot@118.102.131.235 sh pkbot/bin/hubot'
		    
              }
									    }
									    	

