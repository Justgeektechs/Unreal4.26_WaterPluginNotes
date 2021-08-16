# Unreal4.26_WaterPluginNotes

Can you please show us if the ocean mesh can they be resized to fit around a landscape that is 4096 in none of the documents or any tutorials that I’ve seen not 1 mention. I’m totally lost and my scene needs the ocean scene with great-looking realism

Go into “WaterMeshActor”, change “tilesize” to 4096, set “Far Distance Material” to “Water_FarMesh”. The defaults are a bit wonky atm it seems 

##### Is there a way to increase the size of the WaterBodyOcean with the new 4.26 water system?

Yep, I finally found the answer. For anyone who is looking to expand the underwater post processing size here is the answer New 4.26 water questions - #16 by kernelkiller 1. Select your WaterBodyOcean instance go to Collision and change the X,Y of Collision Extents. Now you can have an infinite ocean.

Also to increase surface size. Select your WaterMeshactor > under heading Mesh > increase decrease x,y of Extent in Tiles. By increasing Extent in Tiles and Collision Extents you can make an infinite ocean.

