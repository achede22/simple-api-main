# DevOps Test Task

Hi!

Thanks for taking your time to work on this task.

Ideally this test should take a day, but feel free to take as much time as you need, for us quality means more than speed, although, the latest delivery is five days starting now.

The main goal of this test is for us to get to know about your skills better, as well as for you to get to know our current workflow. The solution of the task is not too hard, so you can focus on technology and scripting, show us what you got :wink:

This is your demo, so overperforming is always very welcome!

## Todo
1. Clone this repository
2. Create a new `dev` branch
3. Please, make sure you use as many commits as you can, we would love to see your progress.
4. After finishing your work, create a Pull Request to `master`.
5. Be ready to answer questions

**Note:** Please keep this coding challenge confidential, don't share any result or code at any public channel, limit your work inside this repo.

## Requirements
 * Keep a clean and understandable folder structure.
 * Document your work, we love comments and documentation.
 * Write all the documentation and comments in English.
 * Use docker and kubernetes.
 
---

## Your tasks:
1. Deploy the services set contained in the repository to production env using Kubernetes.
2. Configure a simple kubernetes cronjob that call both api endpoints every day at 1:00 am.
3. Send component logs to an Elasticsearch instance deployed in the cluster.

## Project description
Simple API is a simple application conformed by 3 main services, the `api-external`, the `api-month` and the `api-day`.
The `api-external` is the entry point and needs to be exposed outside the cluster via the url https://api-external.dev through it you can invoke the 2 services `api-month` and `api-day` that simply print the day of the week and the month in their respective logs. The api call is secured using a secret in the headers.

The endpoints(ENDPOINT_DAY, ENDPOINT_MONTH), ports(PORT) and secret(API_SECRET) must be configured in each kubernetes deployment throught environment variables. Use configmaps and secrets according to the variable type.

## Tip
* You can use minikube to test your work.
* Components can have bugs, they're simple, it shouldn't take long to figure it out.
* You can deploy fluentbit or filebeat and a single elasticsearch instance without kibana, we can view the logs throught elasticsearch REST API.

## Evaluation criteria

This is what we look at - among other things:
* The deployment flow has to run, please provide **short** setup instructions.
* Security.
* Automation.
* Liveness and Readiness of each dependent service.
* Usage of Docker and Kubernetes.

We wish you the best of lucks. :grin:
