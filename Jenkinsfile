    node {

      stage ('Prepare environment') {

//	    git branch: 'master', url: 'https://github.com/shreddy-pk/pkbot.git '
  

	          }

      stage ('Prepare environment') {
//
//		        #sh 'ssh -p2244 -t pkbot@pkbotnode sudo yum install epel-release'
//			      #sh 'ssh -p2244 pkbot@pkbotnode sudo yum install nodejs npm'
			          }

      stage ('Deploy') {

		          sh 'ssh -p2244 pkbot@pkbotnode rm -rf /home/pkbot/pkbot'
              sh 'ssh -p2244 pkbot@pkbotnode git clone -b dev https://github.com/tsrimahesh/pkbot.git'
              sh 'ssh -p2244 pkbot@pkbotnode "cd /home/pkbot/pkbot && npm install "'
					  	sh 'ssh -p2244 pkbot@pkbotnode "cd /home/pkbot/pkbot && npm install hubot-slack --save"'
							sh 'ssh -p2244 pkbot@pkbotnode "export HUBOT_ADAPTER=slack && export HUBOT_SLACK_TOKEN=xoxb-316277351014-4hTDsK3Om2TUOxRhuOa8Jnrd && sh /home/pkbot/pkbot/bin/hubot &"'
//				    sh 'ssh -p2244 pkbot@pkbotnode export HUBOT_SLACK_TOKEN=xoxb-316277351014-4hTDsK3Om2TUOxRhuOa8Jnrd'
//			        sh 'ssh -p2244 pkbot@pkbotnode sh /home/pkbot/pkbot/bin/hubot &'
		    
              }
									    }
									    	

