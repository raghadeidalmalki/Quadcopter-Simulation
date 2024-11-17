# Quadcopter Simulation


This project foocuses on simulating a quadcopter to forecast its behavior. The two subsystems of the model are the airframe and electromechanical subsystems. The airframe encompasses the mechanical structure, while the electromechanical subsystem deals with electrical components and their interactions with the subsystem’s translational and rotational parts. For readability, the system was represented into four main blocks: 
- Torque Command (step block): Sends a command signal to the quadcopter’s motor - can be adjusted interactively so we can observe the immediate impact on the system response.
- Electromechanics Subsystem: Contains the quadcopter’s battery (Panasonic NCA593446), motors (brushless), and propellers. 
- Airframe Subsystem: Contains the quadcopter’s airframe design. 
- Record Block.

Within the airframe subsystem, I added the flight time to assess how long the quadcopter remains in the air which helps in quantifying the impact of the changing parameters. As the time metric shows after applying a thrust force, the quadcopter sustains flight for approximately 22 seconds before it returns to the ground. 
When designing the electromechanical system, I monitored the battery’s state of charge, motor angular velocity, and propeller thrust to understand the model's behavior. Analysis revealed that operating at full power for 9.4 seconds reduced the state of charge by 0.2%, achieving maximum thrust in less than 2 seconds at approximately 0.20 N. 
Additionally, a parameter sweep was conducted to comprehensively characterize the system's behavior, supported by signal logging to track the state of charge, thrust, and RPM signals during simulation. 

For simplicity, these assumptions were made:
- The quadcopter’s motion is one-dimensional. 
- The ground is at x = 0
- The air is still and calm with constant density. 
- The quadcopter always starts from rest on the ground.

![1710762716572](https://github.com/user-attachments/assets/7e72d6ae-398f-41aa-b04a-56d40eab1d86)
  

![1710762715968](https://github.com/user-attachments/assets/66b0184a-047b-4db9-917c-4efe9df01752)


![1710762716024](https://github.com/user-attachments/assets/c246ed09-14fb-4d88-98dc-5f85b0f60878)


![1710762715925](https://github.com/user-attachments/assets/1355b0bc-928a-4172-b523-0a2b36a829d3)


![1710762715303](https://github.com/user-attachments/assets/442bbb2f-e2cb-4658-b0a3-6f34f9d197e4)


![1710762715926](https://github.com/user-attachments/assets/afa95d7d-fa52-4905-87e1-8cc71a858700)


![1710762716216](https://github.com/user-attachments/assets/921c4b69-06f7-497f-b7b9-376f4926cdbf)


![1710762715907](https://github.com/user-attachments/assets/1d89d674-ce8d-4734-98a2-ae179de9baac)


![1710762715903](https://github.com/user-attachments/assets/013229b6-97bd-44ad-95ac-b274590bf5ff)


![1710762715807](https://github.com/user-attachments/assets/f957ff11-1b7f-4182-ab67-ca701dcef893)


![1710762714947](https://github.com/user-attachments/assets/1c01210b-9812-4fb2-bb82-b2f0ed082977)


![1710762715459](https://github.com/user-attachments/assets/4c7edb98-134d-4b1e-afc6-0b853551dfe6)


![1710762715896](https://github.com/user-attachments/assets/653d90f4-1180-4f47-9b3a-9d6993739b13)
