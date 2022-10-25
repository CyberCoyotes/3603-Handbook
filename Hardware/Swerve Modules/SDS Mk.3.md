3603 Bots Utulizing: TAZ, TAZ 2.0 

##
CTRE note: Before you can use any(?) CTRE product, you must
<ul>
    <li>
    <details>   
    <summary>
Install the vendor dependencies for CTRE;
    </summary>
    <ul>
        <li>Open the command palette in VSCode</li>
        <li>Click `Manage Vendor Libraries`, `install online`</li>
        <li>Go online and find the vendor link for CTRE, pasting that into the following prompt.</li>
    </ul>
</details>
</li>
</ul> 
##
# Readying the SDS code template

First; another vendor dependency: throw the url `"https://raw.githubusercontent.com/SwerveDriveSpecialties/swerve-lib/master/SdsSwerveLib.json` into the dependency manager, and things should be merry. also i havent tested it lmao
</br>
After installing the dependencies, you can insert the [template code for SDS].( https://github.com/SwerveDriveSpecialties/swerve-lib/tree/develop/examples/mk3-testchassis/src/main/java/com/swervedrivespecialties/examples/mk3testchassis)
Pay special attention to Drivetrain.java, but use the entire example as a reference.
</br>
Side note, 10/22/22:
Looking into the [Bearbotics code](https://github.com/6391-Ursuline-Bearbotics/2022_UARobotics_Rapid_React), it seems fairly promising. If it's as simple as some basic templating and  