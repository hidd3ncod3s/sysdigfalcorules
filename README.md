# Sysdig Falco Rules

Public Sysdig Falco Rules to protect against known public vulnerabilities. 

## Usage

Enabling it in production machine is as simple checking out the code and modifying the Falco Configuration file once you finished installing Sysdig Falco.
```
  cd /root/
  git clone https://github.com/hidd3ncod3s/sysdigfalcorules.git
```
  
Edit 'rules_file' section of /etc/falco/falco.yaml:

```
rules_file:
 - /etc/falco/falco_rules.yaml
 - /etc/falco/falco_rules.local.yaml
 - /etc/falco/rules.d
 - /root/sysdigfalcorules/rules/
```
