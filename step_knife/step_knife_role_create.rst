.. This is an included how-to. 


To add a role named "role1", enter:

.. code-block:: bash

   $ knife role create role1
   
In the |chef editor| enter the role data in |json|:

.. code-block:: javascript

   ## sample:
   {
      "name": "role1",
      "default_attributes": {
      },
      "json_class": "Chef::Role",
      "run_list": ['recipe[cookbook_name::recipe_name],
                    role[role_name]'
      ],
      "description": "",
      "chef_type": "role",
      "override_attributes": {
      }
   }




When finished, save it.