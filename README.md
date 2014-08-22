Arthur eats bugs! Specifically, it consumes Bugsnag's API to allow you to view project details, errors,
error details etc.

####Installation
    gem install arthur
    
####Initial setup
	Arthur::Api.configure(base_url, auth_token)

####Get project details
	Arthur::Project.fetch(project_id)

####Get project errors
	Arthur::Project.fetch(project_id).errors

####Get error details
	Arthur::Error.fetch(error_id)

####Get error count in environment
	Arthur::Error.fetch(error_id).count_in_environment(env)

####Run tests
    rake

Arthur is released under the MIT License (http://www.opensource.org/licenses/MIT).
