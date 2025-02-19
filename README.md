# Data Science on AWS - Generative AI

Select a branch to explore...

[![Data Science on AWS - O'Reilly Book](img/dsoaws-book.png)](https://github.com/data-science-on-aws/data-science-on-aws/tree/oreilly-book)
[![Data Science on AWS - Generative AI](img/dsoaws-generative.png)](https://github.com/data-science-on-aws/data-science-on-aws/tree/generative)
[![Data Science on AWS - BERT](img/dsoaws-bert.png)](https://github.com/data-science-on-aws/data-science-on-aws/tree/bert)
[![Data Science on AWS - XGBoost](img/dsoaws-xgboost.png)](https://github.com/data-science-on-aws/data-science-on-aws/tree/xgboost)

Based on this O'Reilly book:  

[![Data Science on AWS](img/book_full_color_sm.png)](https://www.amazon.com/Data-Science-AWS-End-End/dp/1492079391/)

## Workshop Description
In this hands-on workshop, we will build an end-to-end AI/ML pipeline to fine tune, evaluate, and deploy a state-of-the-art large language model (LLM) using with Amazon SageMaker and the [Amazon Customer Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/readme.html) which contains 150+ million customer reviews from Amazon.com for the 20 year period between 1995 and 2015.  In particular, we will fine-tune the large language model on the `review_body` column - as well as other columns depending on the language task.

Attendees will learn how to do the following:
* Ingest data into S3 using Amazon Athena, AWS Glue, Spark, Ray and the Parquet data format
* Visualize data with pandas, matplotlib on SageMaker notebooks
* Perform feature engineering on a raw dataset using Scikit-Learn, PySpark, and SageMaker Processing Jobs
* Store and share features using SageMaker Feature Store
* Fine-tune and evaluate a generative AI model using PyTorch and SageMaker Training Jobs
* Evaluate the model using SageMaker Processing Jobs
* Register and version models using SageMaker Model Registry
* Deploy a model to a REST endpoint using SageMaker Hosting and SageMaker Endpoints
* Automate ML workflow steps by building end-to-end model pipelines

## Workshop Instructions
_Note:  This workshop will create an ephemeral AWS acccount for each attendee.  This ephemeral account is not accessible after the workshop.  You can, of course, clone this GitHub repo and reproduce the entire workshop in your own AWS Account._


### 0. Logout of All AWS Consoles Across All Browser Tabs
If you do not logout of existing AWS Consoles, things will not work properly.

![AWS Account Logout](img/aws-logout.png)

_Please logout of all AWS Console sessions in all browser tabs._

### 1. Login to the Workshop Portal (aka Event Engine). 

![Event Engine Terms and Conditions](img/ee1_terms.png)

![Event Engine Login](img/ee-login.png)

![Event Engine Dashboard](img/ee2_team_dashboard.png)


### 2. Login to the **AWS Console**

![Event Engine AWS Console](img/ee3_open_console.png)

Take the defaults and click on **Open AWS Console**. This will open AWS Console in a new browser tab.

If you see this message, you need to logout from any previously used AWS accounts.

![AWS Account Logout](img/aws-logout.png)

_Please logout of all AWS Console sessions in all browser tabs._

Double-check that your account name is similar to `TeamRole/MasterKey` as follows:

![IAM Role](img/teamrole-masterkey.png)

If not, please logout of your AWS Console in all browser tabs and re-run the steps above!


### 3. Launch SageMaker Studio

Open the [AWS Management Console](https://console.aws.amazon.com/console/home)

![Search Box SageMaker](img/search-box-sagemaker.png)

In the AWS Console search bar, type `SageMaker` and select `Amazon SageMaker` to open the service console.

![SageMaker Studio](img/console2_studio.png)

![Open SageMaker Studio](img/console3_open_studio.png)

![Loading Studio](img/studio_loading.png)


### 4. Launch a New Terminal within Studio

Click `File` > `New` > `Terminal` to launch a terminal in your Jupyter instance.

![Terminal Studio](img/studio_terminal.png)


### 5. Clone this GitHub Repo in the Terminal

Within the Terminal, run the following:

```
cd ~ && git clone -b generative https://github.com/data-science-on-aws/data-science-on-aws
```

If you see an error like the following, just re-run the command again until it works:
```
fatal: Unable to create '.git/index.lock': File exists.

Another git process seems to be running in this repository, e.g.
an editor opened by 'git commit'. Please make sure all processes
are terminated then try again. If it still fails, a git process
may have crashed in this repository earlier:
remove the file manually to continue.
```
_Note:  This is not a fatal error ^^ above ^^.  Just re-run the command again until it works._


### 6. Start the Workshop!

Navigate to the `data-science-on-aws/` directory and start the workshop!

_You may need to refresh your browser if you don't see the notebooks._
