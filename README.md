# Player Spline Movement
 This project is a showcase of how to make a player have a movement constrained to a spline.
	
Quick things:
	
1) The level is responsable for letting the player know if this is a splined level or not (free movement or constrained)
2) The only asset created was the BP Spline in the Helping folder.
3) All the movement is handled on the player blueprint.

	3.1) The input coding has been changed to respond to both free movement and spline movement.
4) Currently, the player can only advance while holding D and move back along the spline while holding A. (WiP)
5) Jumping is completely independant from the spline constrains.
6) The player can get locked between meshes, ex. when missing jumps. This is perfect for restricing the player from going backwards in the level and also allows the implementation of death zones.
