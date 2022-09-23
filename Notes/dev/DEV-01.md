# DEV-01, Linking and Appending
### Link:[<>]
#### Tags: []

</br>
</br>

## Linking vs Appending

    Linking When you are linking, you are creating a reference from a source file
    Your actual asset is sitting outside of your current file location. Blender is
    just reading that data from the other file.

    In our current case, BaseFile Blender Project will link to the Max_Rig Blender project

<img src="../images/DEV-01/DEV-01-A1.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-A2.png" width="1100"/>

    The Max object will not really be in our BaseFile scene, but the information of Max
    is being linked in from the Max_Rig blender project. Theres sort of a tether between the files.
    This is generally preferred over appending. 
    Pros for linking are this:
        It keeps your file size small. 
        Any changes in the instanced project file will be reflected on its instances.
        You can also make local changes that wont affect the original

    Therefore do what you can to set up your blender files and folders properly in advance.

    Appending does almost the exact opposite. Appending creates a local copy of the Asset
    inside of your host BaseFile scene. It does this without keeping any reference to the original file

<img src="../images/DEV-01/DEV-01-A3.png" width="1100"/>

    Major Cons for appending
        Your BaseFile scene can get super heavy
        Manually replace assets

</br>
</br>

## Trying it out (Linking)

<img src="../images/DEV-01/DEV-01-B1.png" width="1100"/>
<img src="../images/DEV-01/DEV-01-B2.png" width="1100"/>
<img src="../images/DEV-01/DEV-01-B3.png" width="1100"/>
<img src="../images/DEV-01/DEV-01-B4.png" width="1100"/>

    We have the collection but we cant enter pose mode, only Object mode.
    We need to do a library override in oder to access pose mode

<img src="../images/DEV-01/DEV-01-B5.png" width="1100"/>

    Now able to enter pose mode

<img src="../images/DEV-01/DEV-01-B6.png" width="1100"/>

</br>
</br>

## If you relocated a file and everything breaks (Linking)

<img src="../images/DEV-01/DEV-01-C1.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-C2.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-C3.png" width="1100"/>

    Our mesh is gone! But we can get it back

<img src="../images/DEV-01/DEV-01-C4.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-C5.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-C6.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-C7.png" width="1100"/>

    Max is back

<img src="../images/DEV-01/DEV-01-C8.png" width="1100"/>

    Returning to View Layer

<img src="../images/DEV-01/DEV-01-C9.png" width="1100"/>

</br>
</br>

## Trying it out (Appending)

    Super easy

<img src="../images/DEV-01/DEV-01-D1.png" width="1100"/>

<img src="../images/DEV-01/DEV-01-D2.png" width="1100"/>
