# The-Study-of-Hetero-Dielectric-Buried-Oxide-and-Heterojunction-Dual-Material-TFET


The study aims to enhance the ambipolar behavior and low-ON current of TFETs by proposing and developing a hetero-junction dual material TFET. The addition of the hetero junction to the device aims to reduce the band gap at the source-channel junction and gate oxide, thereby increasing the drain current capacity.

# PROPOSED STRUCTURE:

The proposed structure for enhancing TFET performance is a hetero-junction dual material TFET. This structure incorporates a hetero junction at the source-channel junction and gate oxide, along with a dual material configuration using aluminum (M1) and nickel (M2) as the materials. The gate oxide is made of high-k oxide HfO2 with a K value of 25. This structure is referred to as Hetero Junction Dual Material (HDJM) TFET. The addition of the hetero junction and dual material configuration aims to reduce the band gap at the source-channel junction and gate oxide, resulting in increased drain current capacity and improved performance compared to normal TFETs.

![image](https://github.com/Bhoomi-sravanthi/The-Study-of-Hetero-Dielectric-Buried-Oxide-and-Heterojunction-Dual-Material-TFET/assets/124352354/76920679-1fa0-44de-90d1-0cc5645e378d)

Fig:TCAD simulated Structure

The working principle of the proposed structure with two regions as buried oxide (HfO2 and SiO2) is based on the operation of a Tunnel Field Effect Transistor (TFET). The TFET relies on the principle of band-to-band tunneling of charge carriers between the source and the channel.

In a TFET, the device behavior is determined by the potential applied at the gate terminal (Vgs). When a positive potential is applied, the device behaves as an N-type TFET. The source and drain regions are highly doped with P-type and N-type concentrations, respectively. The source is grounded, while the drain and gate terminals are biased with a positive voltage.

The dominant carriers in an N-type TFET are electrons. The process of dominant carriers entering the channel region is through band-to-band tunneling. As the positive voltage applied at the gate terminal is increased, the bandgap near the source and channel junction decreases. This allows electrons to tunnel from the valence band to the conduction band.

In the ON state of the TFET, when the voltage at the gate terminal is increased, the electrons tunnel from the channel and sweep towards the drain. This results in the flow of current from the source to the drain.

On the other hand, if the voltage at the gate terminal is close to or equal to zero, the device will be in the OFF state. In this state, the conduction band at the channel lies just above the channel valence band due to the band-to-band tunneling mechanism. This leads to a reduction in leakage current.

Overall, the proposed structure operates based on the principles of band-to-band tunneling in a TFET, where the applied voltage controls the flow of electrons from the source to the drain.

# TOOLS USED : 

1.MATLAB:

MATLAB is a software tool used in this study to analyze the characteristics of the proposed TFET structure. It is a programming and numeric computing platform 
widely used by engineers and scientists for data analysis, algorithm development, and modeling. In this project, MATLAB is utilized to study the graph of TFET 
properties with different materials at the dielectric, source, and drain.

  Specifically, MATLAB is used to assess the characteristics of surface potential by varying the thickness of the oxide, with hafnium oxide (HfO2) as the buried 
  oxide. It is also used to evaluate the electric field along the X-axis and Y-axis, representing the lateral and vertical electric fields. Additionally, MATLAB is 
  employed to analyze the drain characteristics by plotting the drain current (Id) versus drain-source voltage (Vds).
  
2.TCAD:
 
TCAD, which stands for Technology Computer-Aided Design, is a computer simulation tool used to develop and improve semiconductor process technologies and devices. 
In the context of this study, TCAD is used to design and simulate the HD-BOX-HJDM-TFET structure and analyze its characteristics. TCAD automates the fabrication 
and operation of semiconductors.

 ATLAS is a particle device simulation tool used in TCAD that predicts the electrical properties of a specific semiconductor structure and provides insights into its physical processes. An ATLAS input data must have five groups of instructions in the correct order: explanation of the structure, specifications for materials and models, definition of a numerical method, specification of the solution, and analysis of the outcomes.

MESH declarations are used to define the mesh structure of the simulation. These declarations specify the location and spacing of the mesh points in the X and Y directions. Each part of the mesh is allocated a region and a material using REGION statements.

Electrode statements define the electrodes in the simulation, such as the gate, source, and drain. These statements specify the location and dimensions of the electrodes.

Doping expressions are used to define the doping concentration in different regions of the structure. These expressions specify the doping concentration and the type of doping (n-type or p-type) in specific regions.

Material statements define the material properties of different regions in the structure. These statements specify parameters such as bandgap and low field mobility.

The METHOD statement specifies the numerical method to be used in the simulation, such as Gummel-Newton.

After running the simulation, the results can be analyzed by examining the runtime output, log files, and structure files. The TONYPLOT tool is used to open and visualize these files.

In summary, TCAD is a powerful tool used in this study to design, simulate, and analyze the characteristics of the HD-BOX-HJDM-TFET structure. It automates the semiconductor fabrication process and provides insights into the device's electrical properties and physical processes.

# WORKING:

The project is divided into two parts: Analytical Modeling in MATLAB and Characteristics Analysis in TCAD.

In the MATLAB implementation, the surface potential of the proposed structure is derived using Poisson's equation and boundary conditions. The steps involve differentiating the surface potential with respect to y, finding unknown values using boundary conditions, calculating the surface potential at the drain-source junction, and differentiating the surface potential to obtain the electric field. The drain current is then designed by solving for the device's surface potential using Kane's model equation for tunneling current.

In TCAD implementation, the code is implemented in DECK BUILD of Silvaco TCAD. The steps involve defining mesh dimensions, specifying different regions and materials, defining electrodes, specifying doping concentrations, defining dual material properties, and solving for the voltages at the source, drain, and gate. The results are then read from the .str and .log files, and further analysis is done using Tonyplot. The results are saved as .csv files and can be compared with the MATLAB outputs.

Overall, the project involves implementing the analytical model in MATLAB to analyze the surface potential, electric field, and drain current, and using TCAD to simulate and analyze the characteristics of the proposed structure.
