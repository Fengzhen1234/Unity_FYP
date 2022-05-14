# Unity Versions

### Install **2021.2.10f1** & **2020.3.161f**
<br>

# Projects

- Racing Game (Unity Tutorial On Vehicle System)
    - [How To Make A Racing Video Game Tutorial](https://youtube.com/playlist?list=PLhWBaV_gmpGXxscZr8PIcreyYkw8VlnKn)

- SUMO UNITY Realtime
    - Generate Simulation Scene solely

- Unity TCP Sumo
    - Sumo Client and other vehicle updation script included

<br>

# SUMO-UNITY

## Overview
![Generated Map From Sumo File](/GeneratedMap.png)

## Assets and Dependencies

- [TraCI library](https://github.com/SvenMertin/SUMO3d)

- [Logitech SDK](https://assetstore.unity.com/packages/tools/integration/logitech-gaming-sdk-6630#description)<br>
**Note**: Version in the store is outdated, LogitechSteeringWheelEnginesWrapper.dll has been replaced<br>

- [Realistic Cars HD](https://assetstore.unity.com/packages/3d/vehicles/land/realistic-car-hd-05-133027#description)<br>

- [City Package](https://assetstore.unity.com/packages/3d/environments/urban/city-package-107224#description)<br>

- [EasyRoads3D Free v3](https://assetstore.unity.com/packages/3d/characters/easyroads3d-free-v3-987#description)<br>

- [Nature Starter Kit2](https://assetstore.unity.com/packages/3d/environments/nature-starter-kit-2-52977#description)<br>

- [SuperSplines](https://assetstore.unity.com/packages/tools/level-design/supersplines-2020#description)<br>

- [Standard Assets (for Unity 2018.4)](https://assetstore.unity.com/packages/essentials/asset-packs/standard-assets-for-unity-2018-4-32351#description)<br>
**Note**: Dependency needed by Realistic Cars HD
<br>


## Scripts
1. PathConstants.cs: paths to all assets used in the scene<br><br>

2. GenerateScene.cs: Unity editor window GUI to initialize simulation scene<br> 
![Unity Editor GUI](/UnityEditorGUI.jpg)<br><br>

3. ImportAndGenerate.cs: Deserializes SUMO files, generate simulation scene based on the files imported<br>
**Note**: important to include **NetFileComponents** in the scripts <br><br>

4. SUMOClient.cs: Establish communications between SUMO and Unity.<br>Suggested Port: **127.0.0.1:4001** <br><br>

5. Input and Car Controller: Find scripts attached to the vehicle prefabs. 


<br>

## Next Step
1. Refine camera script, automate the process of object attaching
2. Fix bugs in SUMOClient.cs, SUMO shuts when TraCI command is passed on to SUMO
3. Refine vehicle script, vehicle motion and rear view mirror<br>
**Note**: you may find the example code in the practice project
