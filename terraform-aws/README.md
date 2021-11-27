# Introducing Infrastructure As Code With Terraform
Introducing Infrastructure As Code With Terraform

#@title Install Terraform
#@markdown 1. Download from https://www.terraform.io/downloads.html
#@markdown 2. unzip
#@markdown 3. set `PATH`
%%bash
curl -so terraform.zip https://releases.hashicorp.com/terraform/0.12.2/terraform_0.12.2_linux_amd64.zip
unzip terraform.zip > /dev/null && rm -f terraform.zip > /dev/null
mv terraform /usr/local/bin > /dev/null
terraform --version

Terraform v0.12.02

%%bash
rm -rf samples
git clone samples

#DEMO: Hello Terraform

%%bash
cd samples/terraform/hello_terraform
terraform apply

##What is IaC?

    Infrastructure as code (IaC) is the process of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.[^1]
    

[^1]Andreas; Wittig, Michael (2016). Amazon Web Services in Action. Manning Press. p. 93
