```terraform init```

Ensure Terraform code is formatted properly:

```terraform fmt```

Ensure code has proper syntax and no errors:

```terraform validate```

See the execution plan and note the number of resources that will be created:

```terraform plan```

Deploy resources:

```terraform apply```

Enter yes when prompted.

After terraform apply has run successfully, you can either use the AWS CLI on the Controller node to list and describe created resources or you can log in to the AWS Console to verify and investigate created resources.

Finally, on the Terraform Controller node CLI, delete all resources which were created and ensure that it runs through successfully.

```terraform destroy```

Moving state in terraform:

```terraform state mv module.condis_cdb.aws_dynamodb_table.condis_table aws_dynamodb_table.dynamodb-table```


Use environment configuration files:

```terraform plan -var-file=terraform.int.tfvars```

Resources:

https://ryaneschinger.com/blog/terraform-state-move/

https://www.hashicorp.com/blog/zero-downtime-updates-with-terraform

https://stackoverflow.com/questions/72456421/migrate-a-dynamodb-table-in-terraform-module-without-destroying-and-recreating-t
