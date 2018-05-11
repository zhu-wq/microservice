#NodeJS Project Creation

	##Author name email and license settings
		npm set init.author.email "zhu.wenqiang@outlook.com" 
		npm set init.author.name "Wenqiang Zhu"
		npm set init.license "MIT"

	##Create the project
		cd ~/
		mkdir NodeJSProjects
		cd NodeJSProjects
		mkdir microservice
		cd microservice
		npm init
		>package name: (microservice)
		>version: (1.0.0)
		>description: Demo project for NodeJS Microservice
		>entry point: (index.js)
		>test command:
		>git repository: git@github.com:zhu-wq/microservice.git
		>keywords: NodeJS Microservice
		>license: (MIT)
		echo "#NodeJS Project Creation" >> README.md

		git URL可以写成这样：

		git://github.com/user/project.git#commit-ish
		git+ssh://user@hostname:project.git#commit-ish
		git+http://user@hostname/project/project.git#commit-ish
		git+https://user@hostname/project/project.git#commit-ish
		**commit-ish 可以是任意tag，hash，或者可以检出的分支，默认是master分支。

	##Git initilization and push to github
		git init
		git add README.md
		###commit to local repo
		git commit -m "project init"
		###create remote repo
		git remote add microservice git@github.com:zhu-wq/microservice.git
		###push to remote and link the local master branch to remote master branch
		git push -u microservice master
		###later we can easily use below command to push the update to github
		git push microservice master

#Starting to learn NodeJS microservice