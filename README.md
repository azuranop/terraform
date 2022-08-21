```terraform init```

Ensure Terraform code is formatted properly:
terraform fmt

Ensure code has proper syntax and no errors:
terraform validate

See the execution plan and note the number of resources that will be created:
terraform plan

Deploy resources:
terraform apply

Enter yes when prompted.

After terraform apply has run successfully, you can either use the AWS CLI on the Controller node to list and describe created resources or you can log in to the AWS Console to verify and investigate created resources.

Finally, on the Terraform Controller node CLI, delete all resources which were created and ensure that it runs through successfully.
terraform destroy
