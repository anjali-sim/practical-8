# Practical-8 using Github Actions

In this, I have deployed my React Practical-4 using Github Actions.

### What is Github Actions?
GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. It helps you automate your software development workflows from within GitHub. In GitHub Actions, a workflow is an automated process that you set up in your GitHub repository.

## :sparkles: Steps to deploy react application using Github Actions
1. First of all , Create a bucket in S3 with the necessary configurations and permissions.

![Screenshot from 2023-06-07 11-30-45](https://github.com/anjali-sim/practical-8/assets/122269010/ee676786-b2aa-4e9b-a1a3-5f8127dffa7e)

![Screenshot from 2023-06-07 11-29-54](https://github.com/anjali-sim/practical-8/assets/122269010/27ece050-9f21-4365-95de-2f0e43c2f440)

2. Enable Static website hosting and apply bucket policy.

![Screenshot from 2023-06-07 11-32-00](https://github.com/anjali-sim/practical-8/assets/122269010/aef3eeb4-88fa-4a5c-8ae9-be919743f9ef)

![Screenshot from 2023-06-07 11-35-56](https://github.com/anjali-sim/practical-8/assets/122269010/9eb8fb00-48a9-467c-936d-745b125af6f9)

3. Create an IAM user and create the access keys and store it.

![Screenshot from 2023-06-07 11-51-20](https://github.com/anjali-sim/practical-8/assets/122269010/14313383-ca6d-45d7-959e-6f6e66faf225)

4. In the Project, create a folder .github and in that create one another folder named workflows and in it create a file called workflow.yml.

5. In the workflow.yml file, add the necessary configurations in it with proper paths.

![Screenshot from 2023-06-08 13-59-27](https://github.com/anjali-sim/practical-8/assets/122269010/b8c21483-fe12-4d58-9315-222b45810779)

6. In the Github account, Go to Settings -> Secrets and variables -> Actions -> New Repository Secret -> then add all the access keys with proper name and value.

![Screenshot from 2023-06-07 17-39-01](https://github.com/anjali-sim/practical-8/assets/122269010/054009aa-4bef-457c-9aeb-61ec13727475)

7. In the Project in VScode, push the changes and in the Github Account, go to Actions and our react application would be deploying.

![Screenshot from 2023-06-07 20-11-56](https://github.com/anjali-sim/practical-8/assets/122269010/6c0b7a82-157f-4eb9-a4f9-1480f021cd86)

8. After the successful deployment, Go to AWS S3 bucket and you will see the files are uploaded.

![Screenshot from 2023-06-08 14-01-05](https://github.com/anjali-sim/practical-8/assets/122269010/4546da24-55ac-4981-9858-683c95951a86)


## :rocket: Deployed Link
http://github-actions-react-app.s3-website.ap-south-1.amazonaws.com/
