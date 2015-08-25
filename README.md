# VPC configuration for hird.io

This is the VPC configuration for my domain hird.io.

Currently there is just one VPC, with public and private subnets in multiple
AZs.

It is managed through a currently closed-source infrastructure-as-code project
of mine and deployed with:

    curl -XPUT --data-binary @vpc.yml \
      -H 'Content-Type: text/yaml' \
      http://service-name/stacks/hird-io-vpc
