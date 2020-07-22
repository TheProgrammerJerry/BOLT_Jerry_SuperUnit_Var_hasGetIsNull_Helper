# BOLT_Jerry_SuperUnit_Var_hasGetIsNull_Helper
A way to simplify handling variables in your BOLT projects.

# Requirements
Requires [BOLT for Unity](https://assetstore.unity.com/packages/tools/visual-scripting/bolt-163802)
Tested on Unity 2019.3.1f1

# Usefulness / Why To Use
This is a Super (heh) powerful Super Unit that I am integrating heavily into my projects. It enforces good usage of variables within BOLT Flows to ensure they are less error-prone by making sure the variables exist and are not null. The Super Unit is pretty flexible and includes variations such as checking for variables on other game objects. This Super Unit also reduces the amount of redundant work you perform when making variables that are less prone to errors.

Below is an example of using the Super Unit versus the vanilla way:
![Example Usefulness](./SS_Graph_Example_Before_After.png?raw=true "Example Usefulness")
The top portion of the graph is using the Super Unit which is flexible and easy to read. The bottom portion is performing similar checks without the Super Unit. There is a lot more work to connect the graph and this is repeated many times if you use many variables. The end result is a much cleaner graph that is less prone to errors.

# Demo Scene
The package includes a demo scene as seen below:
![Demo Scene](./SS_Scene.png?raw=true "Demo Scene")

When you run the scene, each line is testing for a different requirement using the same, or similar Super Units. Each test for example will look for if a variable is existing, or is null. These tasks typically have a lot of redundant logic and this Super Unit reduces that amount of work.

The demo scene is only a small sample of how you could use the Super Unit. You can really use it whenever you are getting a variable in your flows. 

# Bring Into Project (How to use)
I am assuming you have used Unity enough to know how to bring the asset into your project. You would import the unityasset file into your project. From there, you can use the Super Units within your BOLT Flows.

# Included SuperUnity Purposes
JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_Ver00001: This is a base Super Unit that simply allows checking if a Game Object has the variable you gave it. It returns a boolean to let you know if it had the variable, and also the value.

JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_THISOBJECT_Ver00001: A wrapper for JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_Ver00001 Super Unit which simply makes it easier to look for the variable on the object using the Super Unit.


JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_THATOBJECT_Ver00001: A wrapper for JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_Ver00001 Super Unit which simply makes it easier to look for the variable on another game object. This is the same as calling the wrapped Super Unit directly, but is here for readability and to be clear.

JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_NullCheck_Ver00001: Extended version of JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_Ver00001 which also tells you if the variable was null, and if it was existing AND null.

JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_NullCheck_THISOBJECT_Ver00001: Similar to JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_THISOBJECT_Ver00001 but using JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_NullCheck_Ver00001.

JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_NullCheck_THATOBJECT_Ver00001: Similar to JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_THATOBJECT_Ver00001 but using JerryBOLT_V1_SUPERUNIT_HasVariable_GetVal_NullCheck_Ver00001.


# Possible Enhancements
A future enhancement could be to check if the variable equals a certain value. This would reduce the redundant work even further.
