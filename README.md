## Hi (>‿◠)✌

Here's a link to the original repo: https://github.com/hku-mars/fast_lio

"Steps.."

1. Create and build your workspace.

Note: I'm using velodyne.yaml.. so if you wanna change params only edit this file

2. In velodyne.yaml..change the imu topic to the one you're using and also change imu_init_count
3. Also change the extrinsic translation matrix..but dont change the rotation matrix..it will be decided on its own when you input your imu topic

Note:Point(imu)=R*Point(lidar)+T

Note: Fast lio has FLU frame

Note:You don't need to make any other changes

5. Run this command:
   ```
   ros2 launch FAST_LIO mapping.lauch.py
   ```



