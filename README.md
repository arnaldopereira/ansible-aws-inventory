Ansible AWS Dynamic inventory
============================

Install dependencies
--------------------

    mkvirtualenv ansible-aws-inventory
    pip install -r requirements.txt


Make sure boto has access to the required credentials by, for example, exporting them:


    export AWS_ACCESS_KEY_ID='AK123'
    export AWS_SECRET_ACCESS_KEY='abc123'


Runs ping on every instance that matches the AWS tag area:architecture
----------------------------------------------------------------------


    ansible -i ec2.py ping.yml


References
----------

http://docs.ansible.com/ansible/intro_dynamic_inventory.html

http://docs.pythonboto.org/en/latest/boto_config_tut.html
