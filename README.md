# make-terraform

A convenience GNUMakefile that provides shortcuts for using Terraform:
* `make` (a/k/a `make again`) - using environment/Terraform variables or a .env file, apply the configuration (perform init if needed)
* `make valid` - using environment/Terraform variables or a .env file, validate the configuration (perform init if needed)
* `make clean` - destroy the configuration
* `make fresh` - `clean` actions plus delete the log, state files, and provider plugins
* `make neat` - format the .tf files
* `make state` - show what is in the Terraform state
* `make count` - count of the items in the Terraform state

If you prefer to disable color in Terraform's output while using the GNUMakefile, set the environment variable `COLOR_OPTION` to `-no-color`.
