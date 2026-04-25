# AI-Project-Life-Cycle-Chat-Bot
AI Project Life Cycle Chat Bot for Project Managers
# SageMaker AI Life Cycle Monitoring Bot

An automated bridge between **AWS SageMaker** and **Slack** to help AI Project Managers monitor the ML Life Cycle in real-time.

## 🚀 What this monitors:
* **Design/Dev:** Pipeline execution status (Success/Failure).
* **Validation:** New model versions awaiting approval in the Model Registry.
* **Production:** Real-time data and concept drift alerts.

## 🛠️ Setup Instructions
1. **Slack Webhook:** Create an "Incoming Webhook" in your Slack App settings.
2. **Deploy Code:**
   * Zip the contents of the `/src` folder.
   * Upload `lambda_function.zip` to an S3 bucket.
3. **Infrastructure:**
   * Run the CloudFormation template in `/cloudformation`.
   * Provide the `SlackWebhookURL` and `S3BucketName` as parameters.

## 🤖 Example Notification
> 📦 *Model Package Group Update*
> **Model:** Speech-Recognition-v2
> **Status:** Pending Manual Approval
> **Metrics:** Accuracy 0.94 | Latency 40ms
