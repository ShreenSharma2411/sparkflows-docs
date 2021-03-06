WindowRanking
=========== 



Type
--------- 

transform

Class
--------- 

fire.nodes.etl.NodeWindowRanking

Fields
--------- 

.. list-table::
      :widths: 10 5 10
      :header-rows: 1

      * - Name
        - Title
        - Description
      * - partitionByCols
        - PartitionBy
        - partition column names separated by comma(,) 
      * - orderByCols
        - OrderBy
        - order by column names separated by comma(,)
      * - windowFunction
        - Window Function
        - Window Function Name


Examples
---------

Input
--------

.. list-table:: 
   :widths: 20 20 20 20 20 20
   :header-rows: 1

   * - id
     - price
     - lotsize
     - bedrooms
     - bathrms
     - stories
   
   * - 1
     - 42000
     - 5850
     - 3
     - 1
     - 2
   
   * - 2
     - 38500
     - 4000
     - 2
     - 1
     - 1
  
   * - 3
     - 49500
     - 3060
     - 3
     - 1
     - 1
  
   * - 4
     - 60500
     - 6650
     - 3
     - 1
     - 2
     
   * - 5
     - 61000
     - 6360
     - 2
     - 1
     - 1
  
   * - 6
     - 66000
     - 4160
     - 3
     - 1
     - 1
     
   * - 7
     - 66000
     - 3880
     - 3
     - 2
     - 2 
  
     
Parameters
------------

.. list-table:: 
   :widths: 20 60
   :header-rows: 1
   
   * - Name
     - Value
     
   * - PartitionBy
     - bedrooms , bathrms
     
   * - OrderBy
     - lotsize , price desc
   
   * - Window Function
     - Rank
     

Output
--------

.. list-table:: 
   :widths: 20 20 20 20 20 20 20
   :header-rows: 1

   * - id
     - price
     - lotsize
     - bedrooms
     - bathrms
     - stories
     - rank
    
   * - 7
     - 66000
     - 3880
     - 3
     - 2
     - 2
     - 1

   * - 3
     - 49500
     - 3060
     - 3
     - 1
     - 1
     - 1
   
   * - 6
     - 66000
     - 4160
     - 3
     - 1
     - 1
     - 2
     
   * - 1
     - 42000
     - 5850
     - 3
     - 1
     - 2
     - 3
   
   * - 4
     - 60500
     - 6650
     - 3
     - 1
     - 2
     - 4
     
   * - 2
     - 38500
     - 4000
     - 2
     - 1
     - 1
     - 1
         
   * - 5
     - 61000
     - 6360
     - 2
     - 1
     - 1
     - 2
     
     
