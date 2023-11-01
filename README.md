# Serverless Functions into AWS/Azure
Create your functions for both AWS/Azure without restrictions. This is a template for such development.

Based on a library from serverless comunity [Serverless website](https://www.serverless.com) that handles multi-cloud [multicloud library](https://github.com/serverless/multicloud).

Theoretic idea is that you can write function (for example Back-End algorithms and functionalities) such as:
* Fetch data from database
* Calculate and create new objects from existing objects
* Save data, create objects
* Perform filters, lookups and other data modifications

And deploy them to Azure/AWS which ever you prefer. Some functionalities that are based on external dependencies (such as database under specific provider) can be vendor locked. Thus architecture of your application will probably need some categories as which functionalities are general (can be hosted on any cloud) and which are vendor specific (I am looking at you Dynamo DB in AWS).

Multi-tenancy seems like a difficult discipline.
