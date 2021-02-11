# Fraud detection in real time effectively and efficiently within everyone grasp.

Online fraud transactions is becoming increasingly difficult to prevent, this is because cybercriminals have become more sophisticated in their attacks and traditional fraud detection mechanisms have become less effective.
A recent pwc study with more than 5,000 institutions across 99 territories indicates that the reported amount of losses from fraud reached the $42 billion in the past two years.
The 13% of those companies had losses over $50 million and only 56% of them carried out an investigation into their most critical incident.

These figures are indeed alarming, therefore according to Gartner, by 2023, 30% of banking and electronic commerce institutions will include, as a critical requirement, the fraud detection capabilities of providers in more than 75% RFPs, which represents an increase of 25% compared to today.

## What is AWS doing to help the customers in the anti-fraud battle?

On the solutions side, we have two good candidates:

1- The serverless liveness detection [solution](https://aws.amazon.com/blogs/industries/improving-fraud-prevention-in-financial-institutions-by-building-a-liveness-detection-solution/).
2- An advanced fraud detection [solution](https://aws.amazon.com/solutions/implementations/fraud-detection-using-machine-learning/) based on Amazon SageMaker.

In the other hand, AWS made General Available on July 28 a managed fraud detection service: [Amazon Fraud Detector](https://aws.amazon.com/fraud-detector/). 

Let's see how to use Amazon Fraud Detector to achieve similar performance and accuracy to SageMaker's advanced solution without being a machine learning expert. Only the training dataset is required and the service takes care of the rest automatically. 
It is worth mentioning, that to further facilitate implementation by our customers, a Jupyter notebook has been provided with all deployment steps.

An important feature of Amazon Fraud Detector is that it allows the customer to define the outcomes rules visually using the model score along with input variables, which allows the customers to extrapolate to AWS the current business rules engine and combine it with the score of probability of fraud that the model predicts.
It also allows you to combine several models in each transaction and consider each result in the outcome rules. 
All of this happens in a matter of milliseconds so that it can be integrated into an online approval workflow. We achieved 160 TPS out of the box in our tests.

## Get Started

If you want to test the solution yourself, just deploy the next CloudFormation template and click on the Jupyter notebook link in the Outputs tab.

| Region | Stack |
| ---- | ---- |
|US East (N. Virginia) | [<img src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png">](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://fraud-detector-blog-assets.s3.amazonaws.com/frauddetector.yaml&stackName=Fraud-Detector) |
|US West (Oregon) | [<img src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png">](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/review?templateURL=https://fraud-detector-blog-assets.s3.amazonaws.com/frauddetector.yaml&stackName=Fraud-Detector) |
