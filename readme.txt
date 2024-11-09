DayZ Sakhal Oils Rig By EZ Rich & XMC For Console and PC xml json Mods Instructions & Terms Of Use

These files spawn oil rigs, with loot, off the NW and SE Coast of the Sakhal main island, at "4952.83, 12224.41" & "13382.85, 6675.76"

Limited Testing on PC Sakhal Local Server DAYZ Version 1.26 Nov 2024.

Created by AND BIG THANKS TO: EZ Rich ( terrellerich91#2154 on Discord).

AND BIG THANKS TO XMC. 

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml / json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

The DayZ Editor Mod .dze files are included for those who are familiar with the mod & how to create custom objects: sakhal-ez-rich-oil-rig.dze and sakhal-xmc-oil-rig.dze

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "sakhal-ez-rich-oil-rig-objects.json" & "sakhal-xmc-oil-rig-objects.json" from the extracted files to inside the "custom" folder of the mission directory on your server. This file places the structures on your map.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/sakhal-ez-rich-oil-rig-objects.json","custom/sakhal-xmc-oil-rig-objects.json"],
	
	
If you already are calling custom jsons to spawn items, seperate the files like this:

	"objectSpawnersArr": [custom/sakhal-ez-rich-oil-rig-objects.json","custom/sakhal-xmc-oil-rig-objects.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.
	
Next we add loot to the structures by adding the following code snippet to the top of your mapgrouppos.xml file, after <map> 

	<!--ez rich oil rig loot-->
	 <group name="Land_Tank_Big" pos="4957.298340 -2.136219 12304.575195" rpy="0.000000 0.000000 -18.000000" a="108"/>
	<group name="Land_Tank_Big" pos="4957.308594 8.363781 12304.855469" rpy="0.000000 0.000000 9.000000" a="81"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="4890.588379 3.945278 12290.309570" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Construction_Crane" pos="4890.568359 29.242376 12287.640625" rpy="0.000000 0.000000 -132.000000" a="-138"/>
	<group name="Land_Tank_Big" pos="4903.466309 6.555828 12263.819336" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Castle_Wall1_20" pos="4958.888672 23.484285 12314.472656" rpy="179.999939 90.000000 142.499985" a="-52.5"/>
	<group name="Land_Castle_Wall1_20" pos="4943.158691 23.697775 12302.709961" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4927.038574 23.651777 12290.913086" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4910.178711 23.909979 12278.566406" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4893.548340 24.215979 12266.883789" rpy="-0.000050 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4932.028809 23.723181 12221.380859" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4985.168457 23.848577 12277.122070" rpy="-0.000063 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4969.908691 23.879377 12266.100586" rpy="-0.000063 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4954.598633 23.680075 12254.734375" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4900.978516 23.780180 12254.544922" rpy="-0.000050 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4918.718750 23.663778 12267.097656" rpy="-0.000063 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4935.188477 23.546377 12278.809570" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4951.318359 23.664381 12290.448242" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4966.628418 23.447985 12302.071289" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4974.748535 23.449884 12289.018555" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4958.148438 23.614981 12276.900391" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20_nolc" pos="4942.198730 23.518084 12265.203125" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4912.188477 23.701078 12243.050781" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4948.148438 23.958776 12233.201172" rpy="-0.000063 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4923.028809 23.820478 12231.527344" rpy="-0.000063 90.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4938.528809 23.778479 12243.020508" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4927.258789 23.612577 12254.056641" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Construction_Building" pos="4952.598633 32.899162 12295.186523" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Construction_Building" pos="4913.808594 32.363754 12256.093750" rpy="0.000000 0.000000 54.499996" a="35.5"/>
	<group name="Land_Container_1Aoh" pos="4980.978516 26.363775 12296.259766" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Wall1_20" pos="4964.728516 24.140280 12244.833008" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4980.708496 23.851576 12256.254883" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Wall1_20" pos="4994.088379 23.762075 12265.979492" rpy="179.999939 90.000000 144.000000" a="-54"/>
	<group name="Land_Tank_Big" pos="4903.278809 -3.939220 12263.902344" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4903.038086 17.560827 12263.833984" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4957.188477 19.368784 12305.476563" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4931.038574 18.571882 12227.160156" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4930.938477 7.815350 12227.268555" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4930.828613 -3.267292 12227.490234" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4989.268555 -3.910923 12269.149414" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4988.978516 6.648479 12269.171875" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="4989.248535 17.648882 12268.947266" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="4921.758789 7.863781 12268.074219" rpy="0.000000 0.000000 -34.000000" a="124"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="4948.158691 7.863781 12283.304688" rpy="0.000000 0.000000 54.999992" a="35"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="4944.588379 7.863781 12238.125977" rpy="0.000000 0.000000 145.999924" a="-55.9999"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="4971.808594 7.863781 12262.207031" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Construction_Building" pos="4963.998535 32.836349 12260.715820" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="5000.258789 30.338068 12268.076172" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4995.258789 30.602766 12275.004883" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4990.278809 30.582060 12282.048828" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4984.278809 30.441668 12287.626953" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Big" pos="4930.328613 28.799673 12222.704102" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4918.488770 30.562765 12228.041992" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4944.328613 31.036165 12226.282227" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="4951.558594 31.084270 12231.692383" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Construction_Crane" pos="4945.948730 43.943245 12227.094727" rpy="0.000000 0.000000 72.000015" a="18"/>
	<group name="Land_Ship_Big_FrontA" pos="4968.218750 14.963282 12325.452148" rpy="0.000000 0.000000 18.000000" a="72"/>
	<group name="Land_Ship_Big_FrontB" pos="4948.538574 13.363781 12329.229492" rpy="0.000000 0.000000 18.000000" a="72"/>
	<group name="Land_Ship_Big_BackB" pos="4877.528809 11.463779 12317.065430" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Ship_Big_BackA" pos="4893.638672 12.876377 12328.135742" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Ship_Big_Castle" pos="4887.168457 21.349874 12324.015625" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Construction_Crane" pos="4968.758789 43.284248 12280.577148" rpy="0.000000 0.000000 163.999985" a="-74"/>
	<group name="Land_Construction_House2" pos="4958.998535 42.733551 12260.164063" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Aoh" pos="4911.528809 -0.070530 12353.453125" rpy="0.000000 -11.499995 0.000000" a="90"/>
	<group name="Land_Smokestack_Metal" pos="4952.268555 3.658077 12256.722656" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Smokestack_Medium" pos="4957.378418 -1.767921 12258.797852" rpy="0.000000 0.000000 98.999985" a="-8.99998"/>
	<group name="Land_Smokestack_Brick" pos="4941.688477 39.459656 12262.825195" rpy="0.000000 0.000000 -36.499989" a="126.5"/>
	<group name="Land_Smokestack_Brick" pos="4949.518555 53.602959 12261.186523" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_Ground1" pos="4957.488770 27.149778 12326.075195" rpy="-90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4950.948730 26.794981 12321.548828" rpy="-90.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pipe_Big_Ground2" pos="4962.718750 26.929174 12322.751953" rpy="90.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_CornerR" pos="4964.348633 28.990179 12319.791016" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_Ground1" pos="4947.018555 27.175077 12313.894531" rpy="90.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pipe_Big_Ground1" pos="4940.288574 27.485380 12310.381836" rpy="90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4938.188477 27.315878 12302.424805" rpy="-90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4931.368652 27.123075 12298.367188" rpy="90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground1" pos="4922.758789 26.933676 12297.486328" rpy="-90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground1" pos="4916.388672 26.863775 12292.815430" rpy="90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4912.598633 28.001974 12286.282227" rpy="-0.000005 89.918434 -126.999947" a="-143"/>
	<group name="Land_Pipe_Big_Ground2" pos="4905.998535 28.176474 12282.195313" rpy="-0.000005 89.916061 53.999996" a="36"/>
	<group name="Land_Pipe_Big_Ground1" pos="4888.718750 28.973875 12270.515625" rpy="179.999908 -89.955757 -126.999947" a="-143"/>
	<group name="bldr_pipe_big_9m" pos="4885.298340 28.735373 12268.130859" rpy="-90.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_CornerL" pos="4884.448730 26.335676 12265.202148" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Pipe_Big_Ground2" pos="4886.978516 29.427877 12256.625000" rpy="-0.000005 89.916061 143.499924" a="-53.4999"/>
	<group name="Land_Pipe_Big_CornerR" pos="4890.998535 27.964575 12251.846680" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Pipe_Big_BuildL" pos="4899.458496 28.678877 12249.084961" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Pipe_Big_BuildR" pos="4909.098633 29.039373 12235.544922" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Pipe_Big_Ground2" pos="4917.988770 28.091375 12235.379883" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_Ground2" pos="4958.248535 27.118879 12230.400391" rpy="90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4964.668457 27.187078 12235.062500" rpy="-90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4968.278809 27.952780 12241.953125" rpy="-90.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pipe_Big_Ground2" pos="4974.458496 27.899878 12246.698242" rpy="90.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pipe_Big_Ground2" pos="4982.788574 28.095274 12246.408203" rpy="90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Container_1Aoh" pos="4982.948730 26.832281 12247.689453" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Bo" pos="4987.818359 26.748777 12251.317383" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Pipe_Big_Ground2" pos="4989.088379 27.903578 12251.286133" rpy="-90.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_Ground2" pos="4990.988770 29.042578 12258.709961" rpy="-90.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pipe_Big_BuildL" pos="4997.428711 29.657980 12267.779297" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pipe_Big_BuildR" pos="4991.688477 29.713377 12275.645508" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4984.182617 25.466642 12293.789063" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4985.024902 25.461309 12292.670898" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4985.806152 25.462515 12291.568359" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="Land_Construction_House2" pos="4909.868652 42.709351 12267.888672" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Castle_Stairs" pos="4902.178711 31.854862 12280.395508" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Castle_Stairs" pos="4896.608398 4.242588 12305.759766" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Castle_Stairs" pos="4946.568359 18.113382 12211.837891" rpy="0.000000 0.000000 -133.499954" a="-136.5"/>
	<group name="Land_Castle_Stairs" pos="4937.528809 -0.855122 12208.044922" rpy="0.000000 0.000000 -38.500000" a="128.5"/>
	<group name="Land_Castle_Stairs" pos="4938.878418 10.605381 12220.846680" rpy="5.999996 0.000000 42.999985" a="47"/>
	<group name="Land_Container_1Bo" pos="4943.228516 16.357180 12222.493164" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Mo" pos="4943.668457 18.945681 12222.128906" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4953.843262 15.536394 12225.069336" rpy="-0.000000 -0.000000 35.999977" a="54"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4952.839355 15.536394 12224.416992" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4953.138672 15.363783 12225.852539" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4953.704590 16.226393 12225.120117" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4953.615234 16.916395 12225.215820" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4952.805176 16.226397 12224.462891" rpy="0.000000 0.000000 -9.000000" a="99"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4952.018555 15.363783 12225.354492" rpy="0.000000 0.000000 27.000000" a="63"/>
	<group name="Bonfire" pos="4950.818359 71.085190 12262.051758" rpy="0.000000 0.000000 152.999924" a="-62.9999"/>
	<group name="Bonfire" pos="4940.648438 56.641853 12264.106445" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Mil_Tent_Big2_3" pos="4936.968750 27.763777 12269.136719" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Mil_Tent_Big1_2" pos="4918.158691 25.663778 12279.976563" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Mil_Tent_Big2_4" pos="4929.278809 27.763777 12277.669922" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Mil_Tent_Big4" pos="4969.838379 39.663750 12302.801758" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Mil_Tent_Big2_5" pos="4944.918457 17.263781 12242.258789" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Mil_Tent_Big1_4" pos="4943.498535 15.163782 12252.669922" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Mil_Tent_Big1_5" pos="4932.268555 15.163782 12245.686523" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Mil_Tent_Big1_3" pos="4924.668457 15.163782 12254.215820" rpy="0.000000 0.000000 144.500000" a="-54.5"/>
	<group name="Land_Mil_Tent_Big2_2" pos="4931.078613 17.163778 12268.245117" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Mil_Tent_Big1_1" pos="4914.658691 15.163782 12265.907227" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Mil_Tent_Big2_1" pos="4942.398438 17.163778 12288.312500" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="Land_Mil_Tent_Big4" pos="4939.138672 16.363783 12273.735352" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Mil_Tent_Big1_4" pos="4957.118652 15.163782 12270.523438" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Mil_Tent_Big1_3" pos="4962.168457 15.337282 12264.177734" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Mil_Tent_Big1_4" pos="4966.868652 15.163782 12257.822266" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Mil_Tent_Big2_2" pos="4973.438477 17.163778 12272.167969" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Mo" pos="4966.228516 16.357180 12279.844727" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Container_1Mo" pos="4958.088379 16.372084 12286.943359" rpy="0.000000 0.000000 63.000000" a="27"/>
	<group name="Land_Container_1Mo" pos="4956.208496 16.357180 12289.393555" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Mo" pos="4917.138672 16.357180 12277.099609" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="Land_Container_1Mo" pos="4934.908691 16.357180 12235.399414" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Aoh" pos="4943.278809 26.848280 12245.193359" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Bo" pos="4943.388672 29.436781 12245.239258" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Aoh" pos="4939.768555 27.078176 12249.995117" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Container_1Bo" pos="4962.268555 26.699080 12276.588867" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Container_1Mo" pos="4906.828613 39.020256 12252.034180" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Mo" pos="4948.838379 39.492355 12243.127930" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Aoh" pos="4949.668457 39.452354 12246.031250" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Mil_Tent_Big1_4" pos="4958.868652 38.353752 12290.712891" rpy="0.000000 1.000000 144.000000" a="-54"/>
	<group name="Land_Pier_Crane_A" pos="4877.928711 16.593580 12298.549805" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Pier_Crane_B" pos="4875.678711 29.563780 12304.194336" rpy="0.000000 0.000000 -115.000015" a="-155"/>
	<group name="Land_Pier_Crane_A" pos="4983.038574 31.148365 12253.477539" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Pier_Crane_B" pos="4987.118652 43.665451 12256.252930" rpy="0.000000 0.000000 -15.500000" a="105.5"/>
	<group name="Land_Container_1Mo" pos="4950.258789 39.564850 12305.591797" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Bo" pos="4932.708496 -0.351082 12368.702148" rpy="-7.500000 -15.499998 18.000004" a="72"/>
	<group name="Land_Container_1Moh" pos="4924.388672 0.373169 12351.663086" rpy="0.000000 0.000000 45.000000" a="45"/>
	<group name="Land_Container_1Mo" pos="4922.738770 2.165989 12354.853516" rpy="0.000000 -19.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Bo" pos="4918.378418 -0.285030 12356.572266" rpy="0.000000 13.999998 45.000000" a="45"/>
	<group name="Land_Container_1Mo" pos="4884.578613 12.438679 12282.752930" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Mo" pos="4887.048340 12.438679 12285.937500" rpy="0.000000 0.000000 -18.000000" a="108"/>
	<group name="Land_Container_1Mo" pos="4905.538574 12.438679 12284.101563" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Container_1Aoh" pos="4901.318359 14.978781 12279.069336" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4903.908691 11.563778 12283.410156" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4903.828613 11.563778 12284.863281" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4903.878418 12.253780 12284.087891" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4903.028809 11.563778 12284.300781" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4904.568359 14.063780 12281.964844" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4904.938477 14.063780 12283.506836" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4904.718750 14.663782 12282.507813" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4897.628418 32.963760 12277.749023" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4896.418457 32.963760 12276.770508" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4897.238770 33.563751 12277.355469" rpy="0.000000 0.000000 45.000000" a="45"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4897.076172 34.171120 12277.815430" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4896.898438 34.823753 12278.038086" rpy="0.000000 0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Aoh" pos="4894.578613 -0.656040 12314.613281" rpy="0.000000 -21.499996 54.499992" a="35.5"/>
	<group name="Land_Castle_Stairs" pos="4972.278809 18.163782 12328.597656" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Container_1Bo" pos="4964.938477 11.663780 12326.914063" rpy="0.000000 10.999998 -94.499985" a="-175.5"/>
	<group name="Land_Container_1Aoh" pos="4961.708496 11.463779 12321.569336" rpy="25.000000 10.500000 -7.499992" a="97.5"/>
	<group name="Land_Container_1Mo" pos="4962.548340 14.621881 12325.084961" rpy="18.499992 1.500000 35.500000" a="54.5"/>
	<group name="Land_Container_1Bo" pos="4960.768555 44.651649 12278.638672" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Mo" pos="4997.618652 34.563751 12259.481445" rpy="0.000000 13.499992 -46.499985" a="136.5"/>
	<group name="Land_Pipe_Big_BuildL" pos="4954.908691 38.263756 12280.114258" rpy="0.000000 0.000000 -36.000103" a="126"/>
	<group name="Land_Pipe_Big_BuildR" pos="4959.638672 38.263756 12273.556641" rpy="0.000000 0.000000 144.000000" a="-54"/>
	<group name="Land_Smokestack_Brick" pos="4938.258789 36.863747 12268.260742" rpy="179.999908 -88.500015 -142.499985" a="-127.5"/>
	<group name="Land_Wreck_C130J" pos="4929.188477 43.563751 12254.711914" rpy="-7.500000 2.499999 -145.499939" a="-124.5"/>
	<group name="Land_Container_1Aoh" pos="4928.558594 34.969749 12254.735352" rpy="0.000000 0.000000 -53.999996" a="144"/>
	<group name="Land_Container_1Bo" pos="4928.678711 37.463745 12254.884766" rpy="0.000000 0.000000 -53.999996" a="144"/>
	<group name="Land_Container_1Moh" pos="4922.588379 36.863747 12252.774414" rpy="179.999908 89.000244 -125.499954" a="-144.5"/>
	<group name="Land_Container_1Moh" pos="4922.688477 36.863747 12249.498047" rpy="-0.000036 90.000000 44.999996" a="45"/>
	<group name="Land_Container_1Bo" pos="4896.508789 1.161388 12345.640625" rpy="0.000000 -21.499994 53.999996" a="36"/>
	<group name="Land_Container_1Aoh" pos="4899.368652 -0.438011 12349.665039" rpy="0.000000 -16.500000 -35.999996" a="126"/>
	<group name="Land_Castle_Stairs" pos="4940.948730 -1.101521 12336.897461" rpy="0.000000 0.000000 18.000000" a="72"/>
	<group name="Land_Tower_TC6" pos="4891.928711 66.363785 12258.711914" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.989258 41.216805 12257.117188" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4891.507813 41.216805 12258.343750" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.272461 41.216805 12257.871094" rpy="-0.000000 -0.000000 71.999977" a="18"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.975586 41.895287 12258.348633" rpy="-0.000000 -0.000000 53.999969" a="36"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.898438 42.513748 12258.283203" rpy="0.000000 0.000000 45.000000" a="45"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.968750 41.143753 12259.541016" rpy="0.000000 0.000000 -125.999992" a="-144"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4892.268555 41.143753 12258.894531" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4891.518555 41.813751 12259.517578" rpy="0.000000 0.000000 -63.000000" a="153"/>
	<group name="Land_Roadblock_WoodenCrate" pos="4890.398438 41.143753 12260.460938" rpy="0.000000 0.000000 72.000015" a="18"/>
	
	<!-- XMC Oil Rig Loot -->
	
	<group name="StaticObj_Platform1_Block" pos="13371.087891 27.941608 6691.967773" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13362.993164 28.756588 6686.086426" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13362.992188 27.956585 6686.086914" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13419.692383 28.756588 6727.283691" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13419.691406 27.941608 6727.283691" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13411.589844 28.756588 6721.398926" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13411.588867 27.956585 6721.398926" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13403.488281 28.756588 6715.515137" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13403.488281 27.941608 6715.515137" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13395.392578 28.756588 6709.635254" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13395.392578 27.956585 6709.635742" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13381.414063 28.756588 6711.834961" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13381.413086 27.941608 6711.834961" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13373.310547 28.756588 6705.950195" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13373.310547 27.956585 6705.950684" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13365.209961 28.756588 6700.065918" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13365.208984 27.941608 6700.065918" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13357.114258 28.756588 6694.184570" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13357.113281 27.956585 6694.184570" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13413.813477 28.756588 6735.378906" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13413.812500 27.941608 6735.378906" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13405.710938 28.756588 6729.494141" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13405.709961 27.956585 6729.494141" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13397.609375 28.756588 6723.610352" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13397.609375 27.941608 6723.610352" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13389.513672 28.756588 6717.730469" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13389.513672 27.956585 6717.730957" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13425.438477 12.017537 6670.442383" rpy="-0.000000 0.000000 54.905136" a="35.0949"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13407.417969 12.017537 6718.217773" rpy="-0.000000 0.000000 -35.230721" a="125.231"/>
	<group name="Land_Pipe_Big_Ground2" pos="13401.165039 11.833364 6727.394531" rpy="0.000000 0.000000 -35.140606" a="125.141"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13373.629883 9.882483 6694.441895" rpy="179.999924 -0.000005 -34.425007" a="124.425"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13383.714844 9.882483 6679.630859" rpy="179.999908 -0.000005 -34.425003" a="124.425"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13393.859375 9.882483 6664.817871" rpy="179.999893 -0.000005 -34.425003" a="124.425"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13407.817383 9.804973 6717.648438" rpy="179.999924 -0.000005 144.769287" a="-54.7693"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13418.175781 9.804973 6702.985352" rpy="179.999908 -0.000005 144.769287" a="-54.7693"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13428.533203 9.804973 6688.320313" rpy="179.999893 -0.000005 144.769287" a="-54.7693"/>
	<group name="Land_Pipe_Big_CornerL" pos="13434.421875 12.274800 6678.166992" rpy="0.000000 0.000000 54.429577" a="35.5704"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13411.980469 9.889960 6661.008789" rpy="179.999893 -0.000005 -125.094528" a="-144.905"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13424.865234 9.857467 6670.128906" rpy="179.999893 -0.000005 -125.094528" a="-144.905"/>
	<group name="Land_Pipe_Big_CornerL" pos="13401.703125 9.629943 6655.231445" rpy="179.999893 -0.000005 -124.093018" a="-145.907"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13436.713867 20.592022 6676.797852" rpy="179.999924 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13435.271484 20.592022 6678.780762" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13402.228516 20.592022 6652.606934" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13400.825195 20.592022 6654.618164" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13389.687500 20.592022 6670.865723" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13388.283203 20.592022 6672.877441" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13379.487305 20.592022 6685.841309" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13378.083984 20.592022 6687.853027" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13368.447266 20.594524 6701.972656" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13367.042969 20.594524 6703.983398" rpy="179.999893 -0.000005 145.145630" a="-55.1456"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13423.957031 20.592022 6694.856445" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13422.514648 20.592022 6696.839355" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13413.588867 20.592022 6709.472656" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13412.146484 20.592022 6711.455078" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13402.246094 20.592014 6725.655273" rpy="179.999893 -0.000005 144.716049" a="-54.716"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13400.828125 20.592014 6727.655273" rpy="179.999893 -0.000005 144.716049" a="-54.716"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13417.810547 20.592030 6664.954102" rpy="179.999893 -0.000005 -125.509201" a="-144.491"/>
	<group name="StaticObj_Pipe_Big_Support" pos="13419.812500 20.592030 6666.378906" rpy="179.999893 -0.000005 -125.509201" a="-144.491"/>
	<group name="Land_Wall_Gate_Tin6_1" pos="13436.727539 14.993816 6678.633789" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Wall_Gate_Tin6_1" pos="13402.255859 14.918767 6652.880859" rpy="-0.000000 0.000000 143.999893" a="-53.9999"/>
	<group name="Land_Tower_TC2_Mid" pos="13405.787109 -0.145719 6686.422852" rpy="179.999924 -0.000005 179.999924" a="-89.9999"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13390.198242 -0.618512 6706.863281" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13390.205078 -1.903512 6706.880371" rpy="179.999924 -0.000005 144.999969" a="-55"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13401.648438 -0.618512 6690.460938" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13401.654297 -1.903512 6690.478516" rpy="179.999908 -0.000005 144.999969" a="-55"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13411.674805 -0.618516 6719.301758" rpy="0.000000 0.000000 10.119174" a="79.8808"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13411.691406 -1.903512 6719.310059" rpy="179.999893 -0.000005 -169.879684" a="-100.12"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13408.128906 -0.618516 6699.618164" rpy="0.000000 0.000000 10.119174" a="79.8808"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13408.144531 -1.903512 6699.625977" rpy="179.999893 -0.000005 -169.879684" a="-100.12"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13378.487305 -0.618531 6690.066406" rpy="0.000000 0.000000 -81.986343" a="171.986"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13378.478516 -1.903512 6690.082031" rpy="179.999893 -0.000005 98.012672" a="-8.01267"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13398.289063 -0.618531 6687.247559" rpy="0.000000 0.000000 -81.986343" a="171.986"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13398.281250 -1.903512 6687.262695" rpy="179.999893 -0.000005 98.012672" a="-8.01267"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13440.082031 -0.618516 6680.203613" rpy="0.000000 0.000000 99.645798" a="-9.6458"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13440.089844 -1.903512 6680.187012" rpy="179.999893 -0.000005 -80.351929" a="170.352"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13420.369141 -0.618516 6683.586426" rpy="0.000000 0.000000 99.645798" a="-9.6458"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13420.376953 -1.903512 6683.570313" rpy="179.999893 -0.000005 -80.351929" a="170.352"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13401.318359 -0.618531 6656.663086" rpy="0.000000 0.000000 -172.084702" a="-97.9153"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13401.303711 -1.903512 6656.655762" rpy="179.999893 -0.000005 7.912658" a="82.0873"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13404.101563 -0.618531 6676.470703" rpy="0.000000 0.000000 -172.084702" a="-97.9153"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13404.087891 -1.903512 6676.463379" rpy="179.999893 -0.000005 7.912658" a="82.0873"/>
	<group name="Land_Tower_TC3_Red" pos="13412.633789 32.505165 6729.764160" rpy="-0.000000 -0.000000 53.999939" a="36.0001"/>
	<group name="Land_Mil_ControlTower" pos="13358.324219 16.122356 6734.784668" rpy="-0.000000 -0.000000 -124.512733" a="-145.487"/>
	<group name="StaticObj_Cemetery_SmallCross" pos="31413.523438 27.561041 6190.015137" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Guardhouse" pos="13373.484375 9.176272 6711.006836" rpy="-0.000000 0.000000 144.859390" a="-54.8594"/>
	<group name="StaticObj_Wreck_Ship_Big_Lifeboat" pos="13369.211914 3.190207 6764.056152" rpy="179.999893 0.000005 -124.979385" a="-145.021"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="13357.476563 36.940636 6692.767578" rpy="-0.000000 0.000000 -25.469206" a="115.469"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="13361.250000 36.940636 6687.452148" rpy="-0.000000 0.000000 -26.368580" a="116.369"/>
	<group name="Land_DieselPowerPlant_Building" pos="13399.781250 42.813881 6661.021973" rpy="-0.000000 -0.000000 53.709850" a="36.2901"/>
	<group name="Land_Radio_building" pos="13375.384766 36.879471 6693.748535" rpy="0.000000 0.000000 -125.445000" a="-144.555"/>
	<group name="Land_Construction_Building" pos="13417.828125 39.176453 6702.078125" rpy="-0.000000 0.000000 -125.999924" a="-144"/>
	<group name="Land_Pier_Crane_A" pos="13391.420898 37.567650 6719.249023" rpy="0.000000 0.000000 144.287704" a="-54.2877"/>
	<group name="Land_Pier_Crane_B" pos="13389.904297 50.685112 6724.867676" rpy="0.000000 0.000000 -114.713226" a="-155.287"/>
	<group name="Land_Smokestack_Big" pos="13383.447266 61.057442 6680.427734" rpy="-0.000000 0.000000 -125.477196" a="-144.523"/>
	<group name="Land_Container_1Moh" pos="13415.193359 45.859612 6693.751465" rpy="-0.000000 0.000000 -80.214348" a="170.214"/>
	<group name="Land_Container_1Moh" pos="13415.859375 45.859612 6687.513184" rpy="-0.000000 0.000000 -40.107204" a="130.107"/>
	<group name="Land_Container_1Moh" pos="13434.980469 45.902672 6688.961914" rpy="-0.000000 0.000000 22.918390" a="67.0816"/>
	<group name="Land_Mil_Tent_Big1_1" pos="13424.397461 44.610489 6683.980469" rpy="-0.000000 0.000000 -126.768280" a="-143.232"/>
	<group name="Land_Mil_Tent_Big1_3" pos="13429.638672 44.580399 6695.540039" rpy="-0.000000 0.000000 52.709286" a="37.2907"/>
	<group name="Land_Mil_Tent_Big2_4" pos="13392.835938 34.302208 6696.660156" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="Land_Mil_Tent_Big2_5" pos="13396.935547 34.302208 6690.907227" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="Land_Mil_Tent_Big2_3" pos="13388.531250 34.302208 6702.507813" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="Land_Container_1Aoh" pos="13415.849609 41.847122 6717.336914" rpy="0.000000 0.000000 53.214390" a="36.7856"/>
	<group name="Land_Container_1Bo" pos="13409.394531 41.847115 6707.207520" rpy="0.000000 0.000000 36.025616" a="53.9744"/>
	<group name="Land_Container_1Bo" pos="13440.136719 48.879341 6697.653809" rpy="0.000000 0.000000 -107.214355" a="-162.786"/>
	<group name="Land_Container_1Mo" pos="13417.755859 45.859612 6689.125488" rpy="-0.000000 0.000000 -40.107204" a="130.107"/>
	<group name="Land_Container_1Mo" pos="13416.854492 48.444496 6688.374023" rpy="-0.000000 0.000000 -70.330872" a="160.331"/>
	<group name="Land_Container_1Mo" pos="13424.070313 45.865181 6709.160645" rpy="-0.000000 0.000000 -36.814224" a="126.814"/>
	<group name="Wreck_Mi8" pos="13414.058594 46.543976 6700.000977" rpy="-3.355288 1.196545 -80.214371" a="170.214"/>
	<group name="Land_Container_1Bo" pos="13361.900391 9.571033 6722.948242" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Container_1Aoh" pos="13370.419922 9.558898 6721.207031" rpy="-0.000000 0.000000 -126.051056" a="-143.949"/>
	<group name="Land_Container_1Bo" pos="13368.407227 9.571036 6727.347168" rpy="-0.000000 0.000000 108.862343" a="-18.8623"/>
	<group name="StaticObj_Container_1C" pos="13370.095703 12.182210 6723.924805" rpy="0.000000 0.000000 -6.540798" a="96.5408"/>
	<group name="StaticObj_Container_1D" pos="13363.876953 9.618239 6714.269531" rpy="0.000000 0.000000 -73.647995" a="163.648"/>
	<group name="Land_DieselPowerPlant_Tank_Big" pos="13437.890625 35.056534 6674.705078" rpy="0.000000 0.000000 -45.765873" a="135.766"/>
	<group name="Land_Smokestack_Metal" pos="13446.298828 49.341850 6679.805176" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Smokestack_Medium" pos="13379.981445 61.717125 6665.316895" rpy="0.000000 0.000000 144.266190" a="-54.2662"/>
	<group name="StaticObj_Container_1C" pos="13413.961914 41.930252 6692.537109" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Container_1C" pos="13430.277344 41.930252 6693.537109" rpy="-0.000000 0.000000 45.836788" a="44.1632"/>
	<group name="StaticObj_Container_1D" pos="13421.065430 41.944733 6702.285156" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Container_1D" pos="13418.363281 33.930031 6696.584961" rpy="0.000000 0.000000 -51.901478" a="141.901"/>
	<group name="Land_Container_1Bo" pos="13412.962891 37.873940 6693.712891" rpy="0.000000 0.000000 -49.918358" a="139.918"/>
	<group name="StaticObj_Wreck_Ship_Big_FrontA" pos="20467.701172 12.932365 9635.099609" rpy="0.000000 0.999988 -55.050049" a="145.05"/>
	<group name="StaticObj_Wreck_Ship_Big_FrontB" pos="20458.197266 11.429865 9617.473633" rpy="0.000000 0.000000 -55.050045" a="145.05"/>
	<group name="StaticObj_Wreck_Ship_Big_BackA" pos="20426.488281 12.876091 9589.988281" rpy="0.000000 0.000000 -36.858379" a="126.858"/>
	<group name="StaticObj_Wreck_Ship_Big_BackB" pos="20410.396484 11.365412 9578.687500" rpy="0.000000 0.000000 -36.858379" a="126.858"/>
	<group name="StaticObj_Wreck_Ship_Big_Castle" pos="20419.677734 21.547211 9585.359375" rpy="0.000000 0.000000 -36.858337" a="126.858"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13448.125000 36.074837 6670.562500" rpy="0.000000 0.000000 53.667820" a="36.3322"/>
	<group name="Land_Pipe_Big_Ground2" pos="13457.216797 35.890121 6677.018066" rpy="0.000000 0.000000 53.667820" a="36.3322"/>
	<group name="Land_Roadblock_Table" pos="13387.126953 8.748118 6728.498047" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_Table" pos="13386.626953 8.748122 6725.098633" rpy="-0.000000 0.000000 57.295769" a="32.7042"/>
	<group name="Land_Roadblock_Table" pos="13391.832031 8.748122 6729.697754" rpy="-0.000000 0.000000 74.484489" a="15.5155"/>
	<group name="StaticObj_Roadblock_Bags_Curve" pos="13383.593750 8.868724 6731.081055" rpy="-0.000000 0.000000 122.039536" a="-32.0395"/>
	<group name="StaticObj_Roadblock_Bags_EndL" pos="13380.781250 8.797416 6730.791016" rpy="-0.000000 0.000000 63.025299" a="26.9747"/>
	<group name="StaticObj_Roadblock_Bags_Long" pos="13386.423828 8.185107 6732.596680" rpy="-0.000000 0.000000 51.566154" a="38.4338"/>
	<group name="StaticObj_Roadblock_Bags_EndR" pos="13384.435547 8.369353 6728.578125" rpy="-0.000000 0.000000 -171.312180" a="-98.6878"/>
	<group name="Land_Roadblock_Table" pos="13371.197266 8.759936 6710.527832" rpy="-0.000000 0.000000 -35.380108" a="125.38"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13367.406250 8.635543 6721.535156" rpy="0.000000 0.000000 144.812836" a="-54.8128"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13368.650391 8.640544 6721.902832" rpy="-0.000000 0.000000 54.287415" a="35.7126"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13367.855469 9.268046 6721.338379" rpy="-0.000000 0.000000 54.287415" a="35.7126"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13395.142578 8.675288 6731.475098" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13395.062500 8.675288 6732.927734" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13395.111328 9.365287 6732.152832" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13394.261719 8.675288 6732.366211" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13372.041016 8.643046 6736.558594" rpy="0.000000 0.000000 57.437634" a="32.5624"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13372.503906 8.643046 6738.075195" rpy="-0.000000 0.000000 3.437743" a="86.5623"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13372.225586 9.243052 6737.091309" rpy="-0.000000 0.000000 3.437743" a="86.5623"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13371.780273 8.765872 6743.932129" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13374.683594 8.763370 6736.733887" rpy="-0.000000 0.000000 3.151339" a="86.8487"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13374.619141 8.763370 6735.293945" rpy="-0.000000 0.000000 3.151339" a="86.8487"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13374.619141 9.393367 6735.994141" rpy="-0.000000 0.000000 3.151339" a="86.8487"/>
	<group name="StaticObj_ammoboxes_stacked" pos="13380.527344 9.247474 6738.162109" rpy="-0.000000 -0.000000 21.891239" a="68.1088"/>
	<group name="StaticObj_ammoboxes_single" pos="13379.958984 8.959983 6736.783203" rpy="-0.000000 0.000000 22.632168" a="67.3678"/>
	<group name="StaticObj_ammoboxes_single" pos="13379.958984 9.359916 6736.783203" rpy="-0.000000 0.000000 22.632168" a="67.3678"/>
	<group name="StaticObj_Garbage_Pile7" pos="13369.946289 8.908252 6720.904785" rpy="0.000000 0.000000 158.845200" a="-68.8452"/>
	<group name="StaticObj_Garbage_Pile8" pos="13370.871094 8.968188 6721.828125" rpy="0.000000 0.000000 -42.899380" a="132.899"/>
	<group name="StaticObj_Garbage_Pile5" pos="13368.931641 8.747622 6727.181152" rpy="-0.000000 -0.000000 23.132368" a="66.8676"/>
	<group name="StaticObj_Garbage_Pile5" pos="13366.995117 8.747626 6727.915527" rpy="-0.000000 -0.000000 -174.004150" a="-95.9958"/>
	<group name="StaticObj_Garbage_Ground_6m_NoLC" pos="13374.795898 8.385016 6749.100098" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Garbage_GroundSq_5m_NoLC" pos="13378.896484 8.404834 6743.248047" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Garbage_GroundSq_5m_NoLC" pos="13388.706055 8.404838 6728.051758" rpy="-0.000000 0.000000 63.025299" a="26.9747"/>
	<group name="StaticObj_Garbage_GroundSq_5m_NoLC" pos="13366.218750 8.369800 6723.263184" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Garbage_Ground_6m_NoLC" pos="13380.736328 8.383307 6744.290039" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13458.521484 32.726563 6675.212402" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13452.056641 32.726563 6670.517090" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13445.603516 32.726563 6665.823730" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13439.151367 32.726563 6661.134277" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13432.686523 32.726563 6656.438965" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13426.234375 32.726563 6651.745605" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13419.773438 32.726563 6647.048340" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13413.308594 32.726563 6642.353027" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13406.856445 32.726563 6637.659668" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13400.394531 32.726563 6632.964355" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13454.833984 32.726570 6687.225586" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13459.523438 32.726570 6680.757324" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13417.328125 32.726570 6738.917480" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13422.016602 32.726570 6732.448730" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13426.704102 32.726570 6725.991699" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13431.386719 32.726570 6719.535645" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13436.073242 32.726570 6713.066406" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13440.763672 32.726570 6706.612305" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13445.455078 32.726570 6700.148438" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13450.144531 32.726570 6693.679199" rpy="0.000000 0.000000 -125.953110" a="-144.047"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13357.281250 32.726578 6685.653809" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13352.587891 32.726578 6692.119629" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13394.834961 32.726578 6633.986328" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13390.138672 32.726578 6640.451172" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13385.447266 32.726578 6646.903320" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13380.759766 32.726578 6653.357422" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13376.068359 32.726578 6659.825195" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13371.365234 32.726578 6666.276855" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13366.671875 32.726578 6672.737793" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13361.976563 32.726578 6679.202148" rpy="0.000000 0.000000 53.994942" a="36.0051"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13353.594727 32.726540 6697.738281" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13360.063477 32.726540 6702.426758" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13366.521484 32.726540 6707.111816" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13372.976563 32.726540 6711.794434" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13382.635742 32.726540 6718.808594" rpy="0.000000 0.000000 -36.001823" a="126.002"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13385.902344 32.726540 6721.168945" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13392.367188 32.726540 6725.858887" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13398.837891 32.726540 6730.546387" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13405.293945 32.726540 6735.232422" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="StaticObj_Wall_Fen4_8" pos="13411.759766 32.726540 6739.921875" rpy="0.000000 0.000000 144.049973" a="-54.05"/>
	<group name="Land_Container_1Aoh" pos="13454.355469 33.354424 6680.782227" rpy="-0.000000 0.000000 53.714794" a="36.2852"/>
	<group name="Land_Container_1Bo" pos="13449.576172 33.383492 6684.051758" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="Land_Container_1Aoh" pos="13416.825195 33.320122 6679.820313" rpy="0.000000 0.000000 -35.856720" a="125.857"/>
	<group name="Land_Container_1Moh" pos="13400.633789 33.366714 6684.312012" rpy="0.000000 0.000000 -71.999947" a="162"/>
	<group name="StaticObj_Container_2E" pos="13354.490234 10.940143 6722.749023" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="StaticObj_Container_2D" pos="13356.878906 10.936019 6725.166016" rpy="0.000000 0.000000 -18.429720" a="108.43"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13359.615234 8.785827 6741.512695" rpy="-0.000000 -0.000000 55.002670" a="34.9973"/>
	<group name="Land_Roadblock_Table" pos="13387.567383 8.887645 6721.125977" rpy="0.000000 0.000000 -9.000000" a="99"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13399.531250 32.571930 6684.998047" rpy="-0.000000 -0.000000 18.000000" a="72"/>
	<group name="StaticObj_Misc_WoodenCrate_3x" pos="13400.732422 32.982201 6684.345703" rpy="-0.000000 0.000000 -158.563904" a="-111.436"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13400.711914 32.447006 6686.555176" rpy="0.000000 0.000000 -22.892969" a="112.893"/>
	<group name="Land_Mil_Guardhouse1" pos="13376.719727 34.349236 6707.043457" rpy="0.000000 0.000000 -125.524803" a="-144.475"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13372.337891 33.492050 6702.052734" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13372.753906 35.792732 6701.190918" rpy="0.000000 0.000000 -156.321198" a="-113.679"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13371.980469 35.777748 6707.289551" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13370.742188 35.792740 6699.022949" rpy="0.000000 0.000000 -124.378548" a="-145.621"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13369.601563 35.792740 6698.212402" rpy="0.000000 0.000000 -125.094719" a="-144.905"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13369.672852 35.792740 6699.240234" rpy="0.000000 0.000000 -124.951477" a="-145.049"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13370.255859 36.420212 6698.669922" rpy="0.000000 0.000000 -124.951477" a="-145.049"/>
	<group name="StaticObj_Misc_Obstacle_Bridge" pos="13373.571289 35.627151 6703.716309" rpy="-0.000000 -0.000000 53.999996" a="36"/>
	<group name="StaticObj_Misc_Obstacle_Bridge" pos="13373.802734 35.627151 6703.393555" rpy="-0.000000 -0.000000 53.999996" a="36"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13372.601563 36.389130 6709.484863" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13373.810547 36.361649 6710.277344" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13375.539063 35.686211 6711.164063" rpy="0.000000 0.000000 -123.257713" a="-146.742"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13377.441406 35.686218 6710.864258" rpy="0.000000 0.000000 -48.772938" a="138.773"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13377.319336 35.686218 6704.008301" rpy="0.000000 0.000000 -125.693291" a="-144.307"/>
	<group name="StaticObj_Misc_WoodPile2" pos="13359.957031 8.655871 6732.875488" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Misc_WoodPile2" pos="13360.884766 8.655871 6733.530273" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Misc_WoodPile2" pos="13360.443359 8.655879 6733.217773" rpy="179.999954 -0.000005 -125.999992" a="-144"/>
	<group name="Land_Roadblock_Table" pos="13378.027344 36.687462 6698.549316" rpy="-0.000000 -0.000000 54.859428" a="35.1406"/>
	<group name="Land_Roadblock_Table" pos="13382.824219 36.678200 6689.071289" rpy="-0.000000 0.000000 -87.540764" a="177.541"/>
	<group name="StaticObj_Misc_Table_Camp" pos="13377.222656 36.690598 6693.213867" rpy="-0.000022 90.000000 -0.000022" a="90"/>
	<group name="StaticObj_Misc_Table_Camp" pos="13352.207031 8.893935 6737.390137" rpy="179.999908 90.000000 116.974663" a="-26.9747"/>
	<group name="Land_Ladder" pos="13397.226563 41.182716 6673.024902" rpy="-0.000000 0.000000 143.999893" a="-53.9999"/>
	<group name="Land_Container_1Moh" pos="13395.314453 39.583153 6678.942383" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Roadblock_Table" pos="13399.935547 38.764061 6677.077148" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Pipe_Small2_Ground" pos="13354.677734 31.660366 6696.129883" rpy="-0.000000 0.000000 143.999893" a="-53.9999"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13398.549805 38.655037 6678.866211" rpy="0.000000 0.000000 -40.106983" a="130.107"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13385.044922 33.102921 6710.691895" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13383.343750 33.102921 6712.391602" rpy="-0.000000 0.000000 -85.943451" a="175.943"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13383.504883 32.466492 6710.648926" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13384.789063 32.466476 6712.168457" rpy="0.000000 0.000000 -15.516803" a="105.517"/>
	<group name="StaticObj_Container_2D" pos="13400.150391 34.749268 6713.377441" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Container_1Aoh" pos="13398.785156 33.385857 6715.433594" rpy="-0.000000 -0.000000 53.999996" a="36"/>
	<group name="Land_Container_1Bo" pos="13400.960938 33.365791 6726.049316" rpy="-0.000000 -0.000000 9.000000" a="81"/>
	<group name="StaticObj_Garbage_Container2_Open" pos="13390.226563 9.077266 6724.373535" rpy="0.000000 0.000000 -27.000000" a="117"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13434.867188 45.590996 6697.795898" rpy="0.000000 0.000000 -34.162060" a="124.162"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13400.401367 33.106316 6682.190918" rpy="-0.000000 0.000000 15.899641" a="74.1004"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13406.972656 40.876579 6707.448242" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13408.574219 40.876595 6717.342773" rpy="-0.000000 0.000000 52.138992" a="37.861"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13418.982422 44.826553 6715.118164" rpy="-0.000000 0.000000 97.975571" a="-7.97557"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13424.887695 44.826546 6699.421387" rpy="-0.000000 0.000000 138.082382" a="-48.0824"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13413.796875 40.882042 6717.900391" rpy="-0.000000 0.000000 53.571281" a="36.4287"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13413.796875 41.506966 6717.900391" rpy="-0.000000 0.000000 53.571281" a="36.4287"/>
	<group name="StaticObj_Misc_WoodenCrate" pos="13413.347656 40.882042 6718.552734" rpy="-0.000000 0.000000 53.571281" a="36.4287"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13416.582031 40.951538 6699.849121" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13424.832031 40.951546 6696.086914" rpy="-0.000000 0.000000 -28.647816" a="118.648"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13417.924805 40.951546 6693.187012" rpy="-0.000000 0.000000 57.295837" a="32.7042"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13422.744141 40.951546 6684.013672" rpy="-0.000000 0.000000 57.295837" a="32.7042"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13424.246094 40.951530 6683.403809" rpy="-0.000000 0.000000 -5.586304" a="95.5863"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13422.828125 41.550201 6682.687012" rpy="-0.000000 0.000000 -34.377346" a="124.377"/>
	<group name="Land_Container_1Moh" pos="13424.102539 41.867477 6689.173340" rpy="-0.000000 0.000000 -41.682487" a="131.682"/>
	<group name="Land_Roadblock_Table" pos="13408.080078 41.047813 6697.196777" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="Land_Roadblock_Table" pos="13416.888672 41.047813 6705.496094" rpy="-0.000000 -0.000000 111.295639" a="-21.2956"/>
	<group name="Land_Roadblock_Table" pos="13426.097656 44.960564 6700.696777" rpy="-0.000000 -0.000000 53.999985" a="36"/>
	<group name="StaticObj_Misc_Table_Camp" pos="13427.812500 45.045456 6704.984863" rpy="179.999954 -0.000005 179.999954" a="-90"/>
	<group name="Land_Roadblock_Table" pos="13431.589844 45.029823 6689.611328" rpy="-0.000000 0.000000 -45.836617" a="135.837"/>
	<group name="Land_Roadblock_Table" pos="13418.943359 44.963173 6690.193359" rpy="-0.000000 -0.000000 49.272987" a="40.727"/>
	<group name="StaticObj_Misc_Table_Camp" pos="13424.450195 44.907867 6690.482910" rpy="-0.000022 90.000000 -0.000022" a="90"/>
	<group name="StaticObj_ammoboxes_stacked" pos="13424.671875 45.559334 6708.339844" rpy="0.000000 0.000000 -37.432343" a="127.432"/>
	<group name="StaticObj_ammoboxes_stacked" pos="13423.552734 45.559334 6709.829590" rpy="0.000000 0.000000 -37.432343" a="127.432"/>
	<group name="StaticObj_ammoboxes_stacked" pos="13413.425781 45.551842 6694.080566" rpy="0.000000 0.000000 -80.404167" a="170.404"/>
	<group name="StaticObj_ammoboxes_single" pos="13414.796875 45.267395 6693.840820" rpy="0.000000 0.000000 -80.331795" a="170.332"/>
	<group name="StaticObj_ammoboxes_single" pos="13414.796875 45.659897 6693.840820" rpy="0.000000 0.000000 -80.331795" a="170.332"/>
	<group name="StaticObj_ammoboxes_single" pos="13415.721680 45.267395 6693.680664" rpy="0.000000 0.000000 -80.331795" a="170.332"/>
	<group name="StaticObj_ammoboxes_single" pos="13415.721680 45.659897 6693.680664" rpy="0.000000 0.000000 -80.331795" a="170.332"/>
	<group name="StaticObj_ammoboxes_single" pos="13420.731445 46.047173 6691.935547" rpy="0.000000 0.000000 -32.489635" a="122.49"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13416.445313 45.072998 6686.235840" rpy="-0.000000 0.000000 -10.886377" a="100.886"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13414.416016 45.722771 6688.893066" rpy="-0.000000 0.000000 52.425312" a="37.5747"/>
	<group name="StaticObj_Misc_WoodenCrate_3x" pos="13415.406250 45.468178 6687.457031" rpy="-0.000000 -0.000000 48.867329" a="41.1327"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13417.387695 45.072998 6688.548340" rpy="-0.000000 0.000000 -40.107037" a="130.107"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13416.541016 45.072998 6689.563477" rpy="-0.000000 0.000000 -40.107044" a="130.107"/>
	<group name="Land_Roadblock_WoodenCrate" pos="13417.599609 45.072998 6689.585938" rpy="-0.000000 0.000000 -40.107044" a="130.107"/>
	<group name="StaticObj_Misc_WoodenCrate_5x" pos="13425.785156 41.550201 6690.662598" rpy="-0.000000 0.000000 -38.388100" a="128.388"/>
	<group name="StaticObj_Misc_WoodenCrate_3x" pos="13415.406250 41.345589 6687.457031" rpy="-0.000000 -0.000000 48.867329" a="41.1327"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13433.632813 36.074837 6659.904297" rpy="0.000000 0.000000 53.667820" a="36.3322"/>
	<group name="Land_Pipe_Big_Ground1" pos="13424.402344 35.893623 6652.904297" rpy="-0.000000 -0.000000 53.999863" a="36.0001"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="13370.505859 35.397202 6678.515625" rpy="-0.000000 0.000000 -36.475399" a="126.475"/>
	<group name="Land_Sawmill_Illuminanttower" pos="13359.578125 41.967972 6700.471680" rpy="-0.000000 -0.000000 143.524933" a="-53.5249"/>
	<group name="Land_Sawmill_Illuminanttower" pos="13420.609375 41.967979 6649.480957" rpy="-0.000000 -0.000000 -35.849426" a="125.849"/>
	<group name="Land_Sawmill_Illuminanttower" pos="13374.751953 18.181950 6719.729492" rpy="0.000000 0.000000 -35.999981" a="126"/>
	<group name="StaticObj_Road_Sidewalk_Stairs" pos="13377.402344 30.245022 6717.848145" rpy="0.000000 0.000000 -35.999985" a="126"/>
	<group name="StaticObj_Road_Sidewalk_Stairs" pos="13376.517578 30.267529 6717.235352" rpy="0.000000 0.000000 -35.999977" a="126"/>
	<group name="StaticObj_Road_Sidewalk_Stairs" pos="13375.647461 30.287502 6716.627441" rpy="0.000000 0.000000 -35.999996" a="126"/>
	<group name="StaticObj_Wall_PipeFence_8" pos="13377.294922 30.602528 6718.774414" rpy="-39.999992 0.000000 53.819622" a="36.1804"/>
	<group name="StaticObj_Wall_PipeFence_8" pos="13374.846680 30.602528 6716.964844" rpy="-39.999992 0.000000 53.819622" a="36.1804"/>
	<group name="StaticObj_Wall_IndCnc4_Low_Pole" pos="13379.009766 33.209435 6716.440430" rpy="-0.000000 0.000000 -36.094398" a="126.094"/>
	<group name="StaticObj_Wall_IndCnc4_Low_Pole" pos="13376.324219 33.209435 6714.510742" rpy="-0.000000 0.000000 -36.094395" a="126.094"/>
	<group name="Land_Guardhouse" pos="13374.222656 9.668090 6752.033691" rpy="-0.000000 -0.000000 54.716263" a="35.2837"/>
	<group name="Land_Tower_TC2_Base" pos="13421.306641 54.813972 6665.184570" rpy="-0.000000 0.000000 -127.912773" a="-142.087"/>
	<group name="Land_Tower_TC2_Mid" pos="13421.980469 104.393471 6665.037109" rpy="-0.000000 0.000000 -127.768814" a="-142.231"/>
	<group name="Land_Tower_TC2_Top" pos="13422.375977 154.129593 6665.234863" rpy="-0.000000 0.000000 -127.768806" a="-142.231"/>
	<group name="Land_DieselPowerPlant_Tank_Small" pos="13438.106445 43.350533 6674.331543" rpy="-0.000000 0.000000 -25.469206" a="115.469"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13390.369141 8.827579 6729.136719" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_Chair_Camp2" pos="13387.902344 8.615237 6729.820801" rpy="90.000000 0.000000 97.403168" a="-7.40317"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13386.449219 8.819903 6723.669922" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_Chair_Camp2" pos="13351.354492 8.938773 6739.189453" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13387.546875 8.964618 6721.893555" rpy="-0.000000 -0.000000 18.000000" a="72"/>
	<group name="StaticObj_Misc_Chair_Camp2" pos="13371.551758 8.558291 6709.533203" rpy="179.999969 44.000000 179.999969" a="-90"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13376.812500 36.770523 6698.328125" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13377.312500 36.558121 6691.828125" rpy="-90.000000 0.000000 -108.861984" a="-161.138"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13382.218750 36.770531 6689.627441" rpy="-0.000000 0.000000 -126.051109" a="-143.949"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13419.976563 45.020386 6690.397461" rpy="-0.000000 0.000000 39.142475" a="50.8575"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13424.582031 44.723068 6691.897949" rpy="-90.000000 0.000000 39.142506" a="50.8575"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13426.383789 44.723068 6702.298340" rpy="-90.000000 0.000000 39.142506" a="50.8575"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13428.185547 45.120399 6703.698242" rpy="-0.000000 -0.000000 39.142506" a="50.8575"/>
	<group name="StaticObj_Misc_Chair_Camp1" pos="13431.591797 45.640717 6689.692871" rpy="179.999954 46.299801 -137.276993" a="-132.723"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="13382.107422 1.056800 6738.116211" rpy="0.000000 0.000000 144.999969" a="-55"/>
	<group name="Land_Construction_Crane" pos="13451.615234 50.036980 6696.962891" rpy="0.000000 0.000000 -37.454380" a="127.454"/>
	<group name="Land_Castle_Stairs" pos="13374.522461 1.379668 6759.745605" rpy="0.000000 0.000000 143.902222" a="-53.9022"/>
	<group name="Land_Pier_Crane_A" pos="13383.703125 13.705083 6747.405762" rpy="0.000000 0.000000 -126.044060" a="-143.956"/>
	<group name="Land_Pier_Crane_B" pos="13389.312500 26.822811 6748.956543" rpy="0.000000 0.000000 -25.045584" a="115.046"/>
	<group name="Land_Container_1Mo" pos="13373.975586 9.550185 6735.786621" rpy="0.000000 0.000000 4.107001" a="85.893"/>
	<group name="Land_Container_1Mo" pos="13379.917969 9.550185 6736.631348" rpy="0.000000 0.000000 22.106977" a="67.893"/>
	<group name="Land_Container_1Mo" pos="13396.771484 9.550189 6732.166016" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Platform1_Block" pos="13422.595703 28.756588 6655.145508" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13422.594727 27.941608 6655.145508" rpy="179.999924 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13414.492188 28.756588 6649.259277" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13414.492188 27.956585 6649.259277" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13406.391602 28.756588 6643.373535" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13406.390625 27.941608 6643.373535" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13398.295898 28.756588 6637.492188" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13398.294922 27.956585 6637.492188" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Wall_IndCnc4_Low_8" pos="13371.394531 7.409141 6753.940430" rpy="0.000000 0.000000 -35.140285" a="125.14"/>
	<group name="StaticObj_Pier_Wooden1_End" pos="13368.781250 -0.559587 6760.029297" rpy="-0.000000 0.000000 -125.139908" a="-144.86"/>
	<group name="StaticObj_Pier_Wooden1_End" pos="13365.482422 -0.557931 6765.160156" rpy="-0.000000 -0.000000 54.859535" a="35.1405"/>
	<group name="StaticObj_Boathouse_PierL" pos="13361.853516 -3.912835 6753.009766" rpy="0.000000 0.000000 -35.140285" a="125.14"/>
	<group name="StaticObj_Boathouse_PierL" pos="13356.437500 -3.912835 6761.205078" rpy="0.000000 0.000000 -35.140289" a="125.14"/>
	<group name="Land_Container_1Mo" pos="13377.211914 12.097707 6735.911621" rpy="0.000000 0.000000 112.538322" a="-22.5383"/>
	<group name="Land_Container_1Mo" pos="13372.376953 9.550185 6742.904785" rpy="0.000000 0.000000 143.429382" a="-53.4294"/>
	<group name="Land_Tisy_RadarPlatform_Top" pos="13363.681641 1.056800 6724.974121" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="StaticObj_Wall_IndCnc4_Low_8" pos="13374.605469 7.409137 6709.310547" rpy="0.000000 0.000000 144.999969" a="-55"/>
	<group name="StaticObj_Pipe_Small_Stairs" pos="13365.324219 9.043258 6742.697266" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="StaticObj_Pipe_Small_20m" pos="13372.365234 8.820422 6732.323242" rpy="0.000000 0.000000 -35.000000" a="125"/>
	<group name="StaticObj_Pipe_Small_Stairs" pos="13380.205078 9.045756 6721.445313" rpy="0.000000 0.000000 -34.999996" a="125"/>
	<group name="Land_Tank_Big" pos="13413.371094 1.025874 6729.784180" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13413.371094 -9.974095 6729.784180" rpy="179.999908 -0.000005 179.999908" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13413.371094 22.743717 6729.784180" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13413.371094 11.743222 6729.784180" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13362.521484 1.025874 6693.690430" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13362.521484 -9.974095 6693.690430" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13362.521484 22.743717 6693.690430" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13362.521484 11.743222 6693.690430" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13449.707031 1.025874 6679.189453" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13449.707031 -9.974095 6679.189453" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13449.707031 22.743717 6679.189453" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13449.707031 11.743222 6679.189453" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13399.057617 1.025874 6643.287109" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13399.057617 -9.974095 6643.287109" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="Land_Tank_Big" pos="13399.057617 22.743717 6643.287109" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tank_Big" pos="13399.057617 11.743222 6643.287109" rpy="179.999893 -0.000005 179.999893" a="-89.9999"/>
	<group name="StaticObj_Pipe_Small2_Ground" pos="13362.675781 8.087428 6746.145508" rpy="0.000000 0.000000 144.999969" a="-55"/>
	<group name="StaticObj_Pipe_Small2_High_Ground" pos="13382.992188 3.293040 6717.128906" rpy="0.000000 0.000000 144.999969" a="-55"/>
	<group name="Land_Pipe_Big_Ground1" pos="13367.245117 11.837079 6703.354980" rpy="-0.000000 0.000000 145.574799" a="-55.5748"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13373.947266 12.020040 6693.909180" rpy="-0.000000 0.000000 145.574661" a="-55.5747"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13384.111328 12.020040 6679.070801" rpy="-0.000000 0.000000 145.574661" a="-55.5747"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13394.271484 12.020040 6664.252441" rpy="-0.000000 0.000000 145.574661" a="-55.5747"/>
	<group name="Land_Pipe_Big_CornerL" pos="13401.843750 12.277539 6655.204102" rpy="-0.000000 0.000000 145.574799" a="-55.5748"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13412.552734 12.017537 6661.395020" rpy="-0.000000 0.000000 54.905136" a="35.0949"/>
	<group name="Land_Pipe_Big_CornerL" pos="13434.380859 9.599784 6678.111816" rpy="179.999893 -0.000005 144.905045" a="-54.905"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13428.156250 12.017537 6688.857422" rpy="-0.000000 0.000000 -35.230721" a="125.231"/>
	<group name="StaticObj_Pipe_Big_18m" pos="13417.787109 12.017537 6703.533203" rpy="-0.000000 0.000000 -35.230721" a="125.231"/>
	<group name="StaticObj_Platform1_Block" pos="13454.995117 28.756588 6678.696777" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13454.994141 27.941608 6678.696777" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13446.892578 28.756588 6672.810547" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13446.891602 27.956585 6672.810547" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13438.791016 28.756588 6666.924805" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13438.791016 27.941608 6666.924805" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13430.695313 28.756588 6661.043457" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13430.695313 27.956585 6661.043457" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13416.713867 28.756588 6663.235840" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13416.712891 27.941608 6663.235840" rpy="179.999908 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13408.611328 28.756588 6657.349121" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13408.610352 27.956585 6657.349609" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13400.509766 28.756588 6651.463379" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13400.509766 27.941608 6651.463379" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13392.414063 28.756588 6645.582031" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13392.414063 27.956585 6645.582031" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13449.113281 28.756588 6686.787109" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13449.113281 27.941608 6686.787109" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13441.010742 28.756588 6680.900391" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13441.009766 27.956585 6680.900391" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13432.910156 28.756588 6675.014648" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13432.910156 27.941608 6675.014648" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13424.814453 28.756588 6669.133301" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13424.814453 27.956585 6669.133301" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13410.830078 28.756588 6671.328613" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13410.830078 27.941608 6671.328613" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13402.726563 28.756588 6665.442383" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13402.726563 27.956585 6665.442383" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13394.626953 28.756588 6659.556152" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13394.625977 27.941608 6659.556152" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13386.531250 28.756588 6653.674805" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13386.530273 27.956585 6653.675293" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13443.230469 28.756588 6694.879883" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13443.229492 27.941608 6694.879883" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13435.126953 28.756588 6688.993164" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13435.126953 27.956585 6688.993652" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13427.026367 28.756588 6683.107422" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13427.025391 27.941608 6683.107422" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13418.930664 28.756588 6677.226074" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13418.929688 27.956585 6677.226074" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13404.941406 28.756588 6679.436523" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13404.941406 27.941608 6679.436523" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13396.837891 28.756588 6673.550293" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13396.837891 27.956585 6673.550293" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13388.738281 28.756588 6667.664551" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13388.737305 27.941608 6667.664551" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13380.642578 28.756588 6661.783203" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13380.641602 27.956585 6661.783203" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13437.341797 28.756588 6702.987305" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13437.340820 27.941608 6702.987305" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13429.238281 28.756588 6697.101563" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13429.238281 27.956585 6697.101563" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13421.137695 28.756588 6691.215820" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13421.136719 27.941608 6691.215820" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13413.041992 28.756588 6685.333984" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13413.041016 27.956585 6685.334473" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13399.057617 28.756588 6687.537109" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13399.056641 27.941608 6687.537109" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13390.955078 28.756588 6681.650391" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13390.954102 27.956585 6681.650391" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13382.853516 28.756588 6675.764648" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13382.853516 27.941608 6675.764648" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13374.757813 28.756588 6669.883301" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13374.757813 27.956585 6669.883301" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13431.457031 28.756588 6711.085449" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13431.457031 27.941608 6711.085449" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13423.354492 28.756588 6705.200684" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13423.353516 27.956585 6705.200684" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13415.253906 28.756588 6699.315918" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13415.253906 27.941608 6699.315918" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13407.158203 28.756588 6693.434570" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13407.158203 27.956585 6693.434570" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13393.173828 28.756588 6695.639648" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13393.173828 27.941608 6695.639648" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13385.070313 28.756588 6689.753418" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13385.070313 27.956585 6689.753418" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13376.970703 28.756588 6683.867676" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13376.969727 27.941608 6683.867676" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13368.875000 28.756588 6677.986328" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13368.874023 27.956585 6677.986328" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13425.574219 28.756588 6719.185547" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13425.573242 27.941608 6719.185547" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13417.470703 28.756588 6713.301270" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13417.470703 27.956585 6713.301270" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13409.370117 28.756588 6707.416992" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13409.369141 27.941608 6707.416992" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13401.274414 28.756588 6701.537598" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13401.273438 27.956585 6701.537598" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13387.292969 28.756588 6703.739746" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13387.291992 27.941608 6703.739746" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13379.189453 28.756588 6697.854004" rpy="0.000000 0.000000 -35.999973" a="126"/>
	<group name="StaticObj_Platform1_Block" pos="13379.189453 27.956585 6697.854004" rpy="179.999893 -0.000005 144.000000" a="-54"/>
	<group name="StaticObj_Platform1_Block" pos="13371.088867 28.756588 6691.967773" rpy="0.000000 0.000000 -35.999973" a="126"/>
	
Save your changes & upload if you need to.

Restart your server and the new structures will appear immediatly, and then they will slowly stock with loot. If you do a wipe will start to appear immediatly.

At the time of uploading these files you cannot spawn infected zombies over water, so you can't add infected to these locations.

Org Files Created by Your EZ Rich & XMC. For more help files for DayZ come visit us at http://bhaalshad.com 

Thank you and enjoy :)  

Thanks, Rob.



