# terraform-stateserver-py

terraform config
---
````bash
➜  terraform-poc cat main.tf 
terraform {
  backend "http" {
    address = "http://192.168.1.235:5000/terraform_state/4cdd0c76-d78b-11e9-9bea-db9cd8374f3a"
    lock_address = "http://192.168.1.235:5000/terraform_lock/4cdd0c76-d78b-11e9-9bea-db9cd8374f3a"
    lock_method = "PUT"
    unlock_address = "http://192.168.1.235:5000/terraform_lock/4cdd0c76-d78b-11e9-9bea-db9cd8374f3a"
    unlock_method = "DELETE"
  }
}
````

