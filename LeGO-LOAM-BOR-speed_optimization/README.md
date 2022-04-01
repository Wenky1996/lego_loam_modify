# LeGO-LOAM-BOR-Modify
This is a fork of the original [LeGO-LOAM-BOR](https://github.com/facontidavide/LeGO-LOAM-BOR/tree/speed_optimization).

In this version I modified some code in order to run successfully in ubuntu20.04.

1. CmakeLists.txt  was modified 
    * add     
   ``` set(CMAKE_CXX_STANDARD 14) ```
    * add  
    ``` find_package(Boost REQUIRED COMPONENTS timer thread serialization)```
    * delete
    ``` link_directories ```
2. In source code variable frame_id was modified
    * from "/xxx" to "xxx"
3. Add new launch file named  "my_run.launch" that can autoplay rosbag file
