# README #

This repo provides data for the DARPA Subterranean Challenge Urban Circuit, including:

* ground truth data for Artifact types and locations

* point cloud scans of the Alpha and Beta courses at Satsop Business Park in Elma, Washington

* information about the topological network structure of the course (see `network` directory)

### Files ###

* Urban_Artifact_Ground_Truth.xlsx -- Spreadsheet listing each Artifact; its type; and x,y,z location in the relevant DARPA coordinate frame for each course (Alpha / Beta) and configuration (1 / 2).

* Urban_Fiducials_Ground_Truth.xlsx -- Spreadsheet listing reference frame fiducials for each course.

* Urban_Artifact_Map.pdf -- Map of Artifact locations and associated artifact types for the two course configurations in the format <artifact ID><config1 type><config2 type>. 

* data/Urban_Circuit_LowRes_Scan_alpha_LowerFloor.pcd -- Point cloud of the Alpha course lower level, defined in the DARPA Cartesian coordinate frame for the Alpha course.

* data/Urban_Circuit_LowRes_Scan_alpha_UpperFloor.pcd -- Point cloud of the Alpha course upper level, defined in the DARPA Cartesian coordinate frame for the Alpha course.

* data/Urban_Circuit_LowRes_Scan_beta_LowerFloor.pcd -- Point cloud of the Beta course lower level, defined in the DARPA Cartesian coordinate frame for the Beta course.

* data/Urban_Circuit_LowRes_Scan_beta_UpperFloor.pcd -- Point cloud of the Beta course upper level, defined in the DARPA Cartesian coordinate frame for the Beta course.

* `network` -- Directory containing course topology and description.

### Course Visualization in RViz ###

The two courses may be visualized as point clouds with artifact markers using ROS and RViz. This package depends on ROS and the `pcl_ros` package to build. 

To visualize the point clouds and artifact locations, run `roslaunch urban_ground_truth view.launch`. Pass with arguments, e.g., `course:=alpha config:=1` to visualize artifact locations for a particular course and configuration. Course may be `alpha` or `beta`. Config may be `1` or `2`.

### Links ###

* Point Cloud Flythrough
    * Alpha: https://youtu.be/gXl4_R9cOlo
    * Beta: https://youtu.be/KID5LeO39xU

* Course Walkthrough
    * Alpha Configuration 1: https://youtu.be/T5M1zDDZy24
    * Beta Configuration 1: https://youtu.be/Amb1ghx8IRM
    * Alpha Configuration 2: https://youtu.be/mhNAX1dpl84
    * Beta Configuration 2: https://youtu.be/Eejmchll0l8

* Matterport Viewer
    * Alpha: https://my.matterport.com/show/?m=dP4NytELbJB
    * Beta: https://my.matterport.com/show/?m=jUip4QJdeg6

* Matterport Files
    * Alpha: https://subt-challenge.s3.amazonaws.com/urban_circuit/Urban_Circuit_Matterport_Alpha_Course.zip
    * Beta: https://subt-challenge.s3.amazonaws.com/urban_circuit/Urban_Circuit_Matterport_Beta_Course.zip

* High-resolution Course Point Clouds
    * https://subt-data.s3.amazonaws.com/urban_scans/SubT_Urban_Circuit_Alpha_Course_Pointcloud.las.zip (6.4 GB)
    * https://subt-data.s3.amazonaws.com/urban_scans/SubT_Urban_Circuit_Beta_Course_Pointcloud.las.zip (7.8 GB)

### Contact Information ###

If you have any questions or comments about this repository, please contact:

* Ryan Halterman - ryhalt@spawar.navy.mil
* Angela Maio - angela.c.maio.civ@mail.mil
* SubT Challenge Mailbox - SubTChallenge@darpa.mil
    
