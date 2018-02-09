# learn2automate

This is a simple lab to show automation concepts by automating F5 using Ansible

1. dev_op_imperative.yml

      prompt> ansible-playbook dev_op_imperative.yml -e state=present -vvv

  In this exercise, we show:
  
    - it is easy to make Domain Specific Knowledge related mistake
    - tedious to change repetitive variables
  
2. dev_op_imperative_v2.yml

  prompt> ansible-playbook dev_op_imperative_v2.yml -e state=present -vvv

  In this exercise, we show
  
    - how to parameterize repetitive variables by using vars.yml
    - how to use ansible-vault to store credetials
    
  prompt> ansible-playbook dev_op_imperative_v2.yml --ask-vault-pass -e @password.yml -e state=present -vvv
 
 3. dev_op_declarative.yml
 
 prompt> ansible-playbook dev_op_declarative.yml -e state=present -vvv
 
  In this exercise, we show
  
    - how to use F5 iApps application services as declarative approach for automation
    - how F5 iApps help ease of operation in shared environment with multiple application teams
