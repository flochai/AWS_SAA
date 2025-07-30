A File gateway is used to create mount points via NFS (linux) or SMB (Windows) to bridge on-premise file storage and S3. The mount points or shares (max 10) are directly mapped onto an S3 bucket which means that files stored into a mount point are visible as objects into that bucket.

Below is an example of a typical two sites architecture using File gateway: 

<img width="1199" height="565" alt="Pasted image 20250730162257" src="https://github.com/user-attachments/assets/3f6f2d1a-1f47-4c49-9b87-c5a06e4aa688" />


It is possible to make interesting multi-sites architectures using the File Gateway:


<img width="1153" height="597" alt="image" src="https://github.com/user-attachments/assets/4f5ebbce-4488-48e2-a425-6e45cd244268" />

Is is possible to combine File Gateway with Lifecyle: 

<img width="1196" height="565" alt="image" src="https://github.com/user-attachments/assets/543353f3-02f3-4ccb-b086-6616cf62807d" />

