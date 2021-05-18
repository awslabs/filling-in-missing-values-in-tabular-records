# Filling in Missing Values in Tabular Records

Missing data values are common due to omissions during manual entry or optional input. Simple data imputation such as using the median/mode/average may not be satisfactory. When there are many features, we can sometimes train a model to use the existing features to predict the desired feature. This solution uses an “AutoML” offering to train a model, deploy it as an endpoint, and then use this model to make bulk predictions. 

We use a data set of Fleet Inventory data and train a model to predict missing values in a target column.


## Requirements

You will need an AWS account to use this solution. Sign up for an account [here](https://aws.amazon.com/).

## Getting Started

To run this JumpStart 1P Solution and have the infrastructure deploy to your AWS account you will need to create an active SageMaker Studio instance (see [Onboard to Amazon SageMaker Studio](https://docs.aws.amazon.com/sagemaker/latest/dg/gs-studio-onboard.html)). When your Studio instance is *Ready*, use the instructions in [SageMaker JumpStart](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-jumpstart.html) to 1-Click Launch the solution.

The solution artifacts are included in this GitHub repository for reference. Note: Solutions are available in most regions including us-west-2, and us-east-1.

**Caution**: Cloning this GitHub repository and running the code manually could lead to unexpected issues! Use the AWS CloudFormation template. You'll get an Amazon SageMaker Notebook instance that's been correctly setup and configured to access the other resources in the solution.


## Architecture
As part of the solution, the following services are used:

* Amazon S3: Used to store datasets.
* Amazon SageMaker Notebook: Used to preprocess and process the data, and to train the deep learning model.
* Amazon SageMaker Endpoint: Used to deploy the trained model.

![](sagemaker/docs/architecture.png)

## License

This project is licensed under the Apache-2.0 License.


