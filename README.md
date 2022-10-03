# Player Spline Movement
 This project is a showcase of how to make a player have a movement constrained to a spline.
	
Quick things (current setup):
	
1) The level is responsable for letting the player know if this is a splined level or not (free movement or constrained)
2) All the movement is handled on the player blueprint.

	2.1) The input coding has been changed to respond to both free movement and spline movement.
4) ~~Currently, the player can only advance while holding D and move back along the spline while holding A. (WiP)~~<br/>
Update 1. You can now choose the desired Movement Type from inside the player Blueprint. Currently supported:
	- Normal:<br/>
	_Regular in engine movement._
	- Spline Bi-Directional:<br/>
	_Move the character with the directional inputs (working on having the option for Up and Down as well, not just Left and Right)_
	- Spline Point Rotation:<br/>
	_Depending on the rotation of point in the spline, the player will need to hold down the correct directional inputs to continue moving. Works better with locked cameras_
	- Camera Based Movement:<br/>
	_WiP. Whatever direction the camera is facing is now forward_
5) Jumping is completely independant from the spline constrains.
6) The player can get locked between meshes, ex. when missing jumps. This is perfect for restricing the player from going backwards in the level and also allows the implementation of death zones.
