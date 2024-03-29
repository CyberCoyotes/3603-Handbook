====
CTRE
====
In the past our team has used a lot of CTRE products (TalonSRX controllers, TalonFX with Falcons, Pigeon2). 
There are some big changes going from 2023 to 2024 with the release of the Kraken and Phoenix 5 to Phoenix 6 (Pro Licenses) frameworks.



------
Links
------
Assume all links are to official documentation unless otherwise noted

- `Tuner X <https://apps.microsoft.com/detail/9NVV4PWDW27Z?hl=en-us&gl=US>`_ can be downloaded from the Microsoft store
- `LATEST Phoenix 6 Documentation <https://v6.docs.ctr-electronics.com/en/latest/>`_
- `Github Examples of Phoenix 6 <https://github.com/CrossTheRoadElec/Phoenix6-Examples>`_

*See also* `links on motion profiling <https://github.com/CyberCoyotes/Handbook/blob/main/docs/source/controls/motion-profiling.rst>`_.

===========
CTRE Notes
===========

--------------
2023 December
--------------
Mostly using this space to document my noticings and notes. 
We have a working arm with Motion Magic (velocity, accelertation) and limits (Stator Current, Supply Current, Forward Limit, Reverse Limit). See also `2024 Taz 3 <https://github.com/CyberCoyotes/2024-Taz3>`_ repo.

-----------
Randomness
-----------

- `Package com.ctre.phoenix6.configs <https://api.ctr-electronics.com/phoenix6/release/java/com/ctre/phoenix6/configs/package-summary.html>`_.
- `API Migration <https://v6.docs.ctr-electronics.com/en/latest/docs/migration/migration-guide/index.html>`_. "Cheat Sheet"
- `CTRE Example of SwerveWithPathPlanner <https://github.com/CrossTheRoadElec/Phoenix6-Examples/tree/main/java/SwerveWithPathPlanner>`_. Provides a basic example with the Phoenix6 Swerve API integrated with PathPlanner's path following for autonomous movement. There is also a `limelight reference <https://github.com/CrossTheRoadElec/Phoenix6-Examples/blob/main/java/SwerveWithPathPlanner/src/main/java/frc/robot/LimelightHelpers.java>`_.

.. list-table:: Control Request Changes
    :widths: 50 50
    :header-rows: 1

    *   - PREVIOUSLY
        - PHOENIX 6
    *   - Position
        - PositionDutyCycle
    *   - Velocity
        - VelocityDutyCycle
    *   - MotionMagic
        - MotionMagicDutyCycle
    *   - Closed-loop + Voltage Compensation
        - {ClosedLoop}Voltage
    *   -
        - {ClosedLoop}TorqueCurrentFOC (requires Pro)

*See also* `API Migration <https://v6.docs.ctr-electronics.com/en/latest/docs/migration/migration-guide/index.html>`_.

~ This is the way.
