# AWS S3 Lambda Data Pipeline 🚀

## 📌 Business Requirements

**Project 1**

1. We have an **S3 bucket** where employee data files will arrive on an hourly basis.  
2. We need a **data pipeline** that is automatically triggered whenever a new file is uploaded to the bucket.  
3. The pipeline should **read the employee data** and **aggregate the salary data** based on the country.  
4. The aggregated data should be **stored back** into a designated S3 bucket.

---

## 🗂️ Overview

This project demonstrates an end-to-end **AWS Data Engineering pipeline** using:
- **Amazon S3**
- **AWS Lambda**
- **AWS IAM**
- **AWS CloudWatch**

It shows how to automate the processing of incoming files, run aggregations, and write the results back to S3 using serverless architecture.

---

## 📁 Project Structure

project/
├── lambda_function.py # Lambda function code
├── requirements.txt # Python dependencies (if any)
├── input/ # Example input files (optional)
├── output/ # Example output files (optional)
└── README.md # Project documentation


---

## ⚙️ How It Works

1. **Upload** your input file to the **S3 bucket** (files arrive hourly).  
2. An **S3 event trigger** automatically invokes the **Lambda function**.  
3. **Lambda** reads the file, aggregates the salary data by country, and writes the output to another S3 bucket or prefix.  
4. Logs are captured in **AWS CloudWatch** for monitoring and troubleshooting.

---

## 🛠️ AWS Services Used

| Service       | Purpose                                          |
|---------------|--------------------------------------------------|
| **S3**        | Store input and output data files                |
| **Lambda**    | Serverless compute to process files automatically |
| **IAM**       | Manage access permissions securely               |
| **CloudWatch**| Monitor logs and Lambda invocations              |

---

## ▶️ Steps to Deploy and Test

1. **Deploy Lambda Function**
   - Upload `lambda_function.py` in the AWS Lambda console.
   - Configure an **S3 Trigger** for the Lambda function.

2. **Test the Pipeline**
   - Upload an employee data file to your S3 bucket.
   - Verify that the output file with aggregated salary data appears in the destination S3 location.
   - Check logs in **CloudWatch** to monitor execution and troubleshoot if needed.

---

## 🤝 Contributing

Pull requests are welcome!  
For major changes, please open an issue first to discuss what you’d like to change or improve.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## ❤️ Support

If you found this helpful:
- ⭐️ Star this repository
- 🍿 Share it with others
- 💬 Feel free to open issues or suggest improvements!

---

> *#AWS #DataEngineering #Serverless #S3 #Lambda*
