# InstanceFusion

We present a robust real-time system to detect, segment, and reconstruct instance-level 3D objects of indoor scenes with a hand-held RGBD camera, namely InstanceFusion. It combines the strengths of deep learning and the traditional SLAM techniques to produce visual compelling 3D semantic models. The key success comes from our novel segmentation scheme and efficient data structure. For each incoming RGBD frame, we take the advantages of the 2D features, 3D point cloud and the fused model to segment out instance-level objects. The corresponding RGBD data along with the instance ID are then fused to the surfel model. In order to sufficiently store and update these data, we design and implement a new data structure based on the CUDA Language. Experimental results show that our method advances the state of the art in instance segmentation and data fusion by a large margin. And the instance segmentation in turn improves the precision of 3D reconstruction. Our system runs 20Hz on a GPU which will support a number of robotic applications such as navigation, manipulation and grasping.  
