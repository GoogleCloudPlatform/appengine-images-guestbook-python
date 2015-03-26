## Guestbook With Images

This is a version of the guestbook sample app for Google App Engine that excersices the [images Python API](https://cloud.google.com/appengine/docs/python/images/usingimages).

See our other [Google Cloud Platform github
repos](https://github.com/GoogleCloudPlatform) for sample applications and
scaffolding for other python frameworks and use cases.

## Project setup, installation, and configuration

## Run Locally
1. Install the [App Engine Python SDK](https://cloud.google.com/appengine/downloads).
See the README file for directions. You'll need python 2.7 and [pip 1.4 or later](http://www.pip-installer.org/en/latest/installing.html) installed too.
1. Clone this repo with

   ```
   git clone https://github.com/GoogleCloudPlatform/appengine-images-guestbook-python.git
   ```
1. Install dependencies in the project's lib directory.
   Note: App Engine can only import libraries from inside your project directory.

   ```
   cd appengine-images-guestbook-python
   pip install -r requirements.txt -t lib
   ```
1. Run this project locally from the command line:

   ```
   dev_appserver.py .
   ```

Visit the application [http://localhost:8080](http://localhost:8080)

See [the development server documentation](https://cloud.google.com/appengine/docs/python/tools/devserver)
for options when running dev_appserver.



## Testing

How do I run the project's automated tests?

* Unit Tests

* Integration Tests


## Deploying
To deploy the application:

1. Use the [Cloud Developer Console](https://console.developer.google.com)  to create a project/app id. (App id and project id are identical)
1. Use the [Admin Console](https://appengine.google.com) to view data, queues, and other AppEngine specific administration tasks.
1. [Deploy the
   application](https://cloud.google.com/appengine/docs/python/tools/uploadinganapp) with

   ```
   appcfg.py -A <your-project-id> --oauth2 update .
   ```

   OR
   Use the google [gcloud CLI](https://cloud.google.com/sdk/gcloud/) to deploy your app:
   ```
   gcloud auth login # only necesssary once
   gcloud config set project <your-project-id> # only necessary once
   gcloud preview app deploy .
   ```



   OR on supported platforms, use the GoogleAppEngineLauncher GUI tool to deploy your app.
1. Congratulations!  Your application is now live at your-app-id.appspot.com

### How to setup the deployment environment

* Addons, packages, or other dependencies required for deployment.
* Required environment variables or credentials not included in git.
* Monitoring services and logging.

### How to deploy


## Troubleshooting & useful tools

### Examples of common tasks

e.g.
* How to make curl requests while authenticated via oauth.
* How to monitor background jobs.
* How to run the app through a proxy.


## Contributing changes

* See [CONTRIBUTING.md](CONTRIBUTING.md)


## Licensing

* See [LICENSE](LICENSE)
