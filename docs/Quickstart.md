:bulb: Before you start, please make sure you did all steps before, which are explained in [Installation](docs/installation.md).


## Preparing

JiggleGen uses Vertexgroups to mask the areas that are supposed for the simulation. Therefore we need to define these areas first in the target mesh and give them a suitable name.

1. Create a Vertexgroup and give it a Name
2. Go to 'Weight Paint Mode' and define the areas that you want to use for the simulation
<img src="/img/vertexgroups_01.jpg" alt="Weightpainting" width="600">

4. While in Weight Paint Mode, alsways use 'Subtract' to erase parts of the VertexGroup selection. Otherwise you will generate empty areas. You can check it by using the 'Zero Weights' view in the upper right corner.
<img src="/img/vertexgroups_02.jpg" alt="Installationsdialog" width="400">

The result should look like this:

<img src="/img/vertexgroups_03.jpg" alt="Installationsdialog" width="600">


## Generating

1. Choose the target Object and Add it to the Batch list.
2. Open the Entry inside the list and select the desired Vertex Group. Press the 'Plus' Icon.
3. Choose a Preset or leave it Empty, to use the current values from the Simulation Settings Area.
4. Press `Generate Cloth`
5. If you want to generate a 'Collision Mesh' from the unselected areas, activate `Add Collision` for the desired Entries and press `Generate Collision`


<img src="/img/batch_03.jpg" alt="Installationsdialog">

Once you hit 'Generate', it generates one ore more Proxy Meshes from the chosen vertex groups. Your Source/Target Mesh will now be mapped to that Proxy Mesh via a 'Surface Deform' Modifier. All proxy meshes are stored in the collection “JiggleGen Physics”.

If you want to refine or regenerate the setup, enable Overwrite and tweak the parameters in the Simulation Settings sub-panel.

Important notes:

* Every batch entry always uses the currently selected preset.

* If no preset is selected, JiggleGen will use the values set directly in the sub-panel.

* If a preset is selected and you want to change these settings: Load it in 'Simulation Settings' Sub-Panel > Adjust the Values as you like > Save it.
