up:
	terraform apply --auto-approve -var environment=${ENV}

down:
	terraform destroy --auto-approve -var environment=${ENV}

init:
	terraform init -backend-config="key=state/${ENV}.tfstate" -backend-config="dynamodb_table=RMIT-locktable-lxnq6o" -backend-config="bucket=rmit-tfstate-lxnq6o"
