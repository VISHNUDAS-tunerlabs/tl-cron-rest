# tl-cron-REST
Service to schedule jobs, Based on Agenda npm package. 
tl-cron-rest

Service to schedule jobs, Based on Agenda npm package. 

Provide your job REST endpoint and it’s scheduling is offered as a service. Introduce a job url, name it, give contact name and email id of person related to the job. sl-agenda-rest will schedule the job for you on specified time and if any error occurs details will be shared to the specified email id.

API Documentation

GET:

api/jobs :// List all job definitions from the database.

POST:

api/jobs :// Add new job definitions.
		   	    // data required:{name,url,person_name,email}

api/jobs/now : // Schedule a defined job for immediate call(now).  

api/jobs/every : // Schedule job for specified intervals, for repeat calls.

api/jobs/once :// Schedule job for a specified time.
	
api/jobs/cancel :// cancel all scheduled jobs if no name specified or cancels job/jobs on specified name (does not remove definitions created by -POST api/jobs)

PUT:

api/jobs/:jobname :// Update job definition.

DELETE:

api/jobs/:jobname :// Delete specified job’s definition and instances.

	
			    

	
	

