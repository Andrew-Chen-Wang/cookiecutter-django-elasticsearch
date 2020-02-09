Elasticsearch
=============

You are provided two cloud hosting options: Elastic Cloud and AWS Elasticsearch

We prefer Elastic Cloud with pricing and better maintenance. We advise against self-hosting EC2 instances for Elasticsearch until your stack is ready to be maintained by separate, dedicated people.

If you're using Elastic Cloud while hosting your server on an AWS EC2 instance, make sure your instance's regions are the same; otherwise, you will be charged :sup:`[1]`.

If you're using Elastic Cloud, `here is their pricing`_ which explains how their pricing categories works. `This is their list of prices`_.

When you create a new deployment, you will be given a username and password. (Username is usually Elastic). Set those in the environment file (``.env/production/.django``).

In the dashboard (the deployment's name on the left side menu), copy the Elasticsearch endpoint and paste into the environment file.

[1]: https://forums.aws.amazon.com/message.jspa?messageID=326076

.. _here is their pricing: https://www.elastic.co/blog/elasticsearch-service-data-transfer-and-snapshot-storage-pricing
.. _This is their list of prices: https://www.elastic.co/blog/elasticsearch-service-on-elastic-cloud-introduces-new-pricing-with-reduced-costs
