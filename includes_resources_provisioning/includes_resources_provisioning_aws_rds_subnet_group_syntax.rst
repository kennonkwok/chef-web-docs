.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


A ``aws_rds_subnet_group`` resource block manages subnets for relational databases. For example:

.. code-block:: ruby

   aws_rds_subnet_group 'db-subnet-group' do
     db_subnet_group_description 'description'
     subnets ['subnet', 'subnet2.aws_object.id' ]
   end

The full syntax for all of the properties that are available to the ``aws_rds_subnet_group`` resource is:

.. code-block:: ruby

   aws_rds_subnet_group 'name' do
     description                   String
     subnets                       String, Array, AwsSubnet, AWS::EC2::Subnet
   end

where 

* ``aws_rds_subnet_group`` is the resource
* ``name`` is the name of the resource block
* ``description`` and ``subnets`` are properties of this resource, with the |ruby| type shown. |see attributes|
