## ex.11.1 Warming up. Let us assume that the application is coded with some other language than JavaScript/TypeScript that you do not know much yourself.

1. CI setup include linting, testing, and building for ruby
	In the continuous integration (ci) setup for Ruby project that I didn't know what ruby is before.
	
        Tools that I might use for linting is RuboCop, in testing is RSpec, and in building, maybe ruby have no build step. 
	Steps
    1.  create configuration file in the ci service, such as .gitlab-ci.yml in gitlab, 
	  2.  define pipeline that tell what runner will do in each stage the stages is like build, test, and deploy.
			1.  check out the code in repository
			2.  set up running environment
			3.  install ruby version and gems
			4.  install project dependency
			5.  set up database
			6.  compile assets to run application
			7.  run test
			8.  ready to deploy, can config ci service to deploy after the build is successful and tested.

2. alternative  CI besides Jenkins and GitHub Actions?
    
        Besides Jenkins and GitHub Actions I would choose ci service such as CircleCI GitLab
		 
3. Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?
	
        Because these cloud-based service also integrate with github repository and supported the language. I think it suit me who just learn about ci and ruby 1 hour ago.